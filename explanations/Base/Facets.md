# Facets and ExtendedFacets
[Facet Information Model Description](../../information_model/Base/Facet.md)
[ExtendedFacet Information Model Description](../../information_model/Base/Facet.md)

# Important!

This is my interpretation of how the Information Model describes Facets. As far as I can tell, absolutely no implementation of SDMX actually does this. See the Notes for what they actually seem to do.

Also, note that I don't talk about ExtendedFacets much here. This is because they are exactly the same as Facets, but add the ability to specify XHTML.

## Description

The Facet is used to describe a range of acceptable values **without** using an ItemScheme. So, essentially you're going to want to use it when you don't have a list of values, but need some other way to describe them. For example, you might want to allow all numbers greater than 0. That's obviously not going to be doable with a Codelist, so you'll need to use Facets.

Why do I say "use Facets" instead of "use a Facet"? That's because you may need to use multiple Facets to define your set of allowable values. First let's look at one Facet. Each individual Facet lets you specify a *facetType*, a *facetValue* and a *facetValueType*. But what do they mean?
- **facetValueType**: This is constrained by the FacetValueType enumeration (with entries like "string", "double" and "inclusiveValueRange"). This provides the basic format we're allowing. For example, by setting it to "integer" we've already said that we'll only accept values that are valid integers.
- **facetType**: Constrained by the FacetType enumeration, this, along with the *facetValue* lets us further constrain the format we specified in the *facetValueType*. For example, you can choose something like "minLength" for *facetType*. This means that *facetValue* should be a positive integer, and that it gives us the minimum length of a FacetValueType that has characters (like "string" or "alphaNumeric").
- **facetValue**: What this attribute means depends almost entirely on what *facetType* was set to. Also worth noting that although this is technically a string, what it's **actually** allowed to be depends on what we set *facetType* to. For example, if *facetType* is "startTime", then *facetValue* needs to be a Date. You can tell what you need to provide by looking at the [FacetType](../../information_model/Base/FacetType.md) page.

Something to notice is that you can only provide one *facetType*-*facetValue* pair per Facet. This means that if you wanted to provide both a minimum length and a maximum length for a string format for example, you can't do it with only one Facet. **This** is why you have the ability to use multiple Facets. Now I couldn't find anything explicitly stating it in the Information Model, but I'm almost 100% certain that you can't vary *facetValueType* within a set of Facets. It wouldn't make much sense to start with "string" and then go to "integer". You should be describing the same basic format the whole way through. I suspect this is why no implementation of SDMX actually uses Facets directly how they're described in the Information Model.

## Examples

You want to allow any string that starts with a capital letter:
```javascript
[
    {
        "facetValueType": "string",
        "facetType": "pattern",
        "facetValue": "^[A-Z].*$"
    }
]
```
We use the base type "string" and then use the "pattern" *facetType* to provide a regular expression describing what we want; in this case that the string starts with any capital letter.

You want to allow any integer between -6 and 103 (don't ask me why):
```javascript
[
    {
        "facetValueType": "integer",
        "facetType": "minValue",
        "facetValue": "-6"
    },
    {
        "facetValueType": "integer",
        "facetType": "maxValue",
        "facetValue": "103"
    }
]
```
Here we needed to provide two Facets, one to establish the minimum value and one to establish the maximum value. Note that at no point did we state that the range is inclusive. This is because that's the default.

You want to allow any integer between but not including -6 and 103:
```javascript
[
    {
        "facetValueType": "exclusiveValueRange",
        "facetType": "minValue",
        "facetValue" : "-6"
    },
    {
        "facetValueType": "exclusiveValueRange",
        "facetType": "maxValue",
        "facetValue": "103"
    },
    {
        "facetValueType": "exclusiveValueRange",
        "facetType": "decimals",
        "facetValue": "0"
    }
]
```
This is very clunky. We use the "exclusiveValueRange" *facetValueType* to specify that neither end of the range is included in the range. However, I believe in the standard (and **definitely** in the SDMX-ML implementation) that "exclusiveValueRange" implies doubles, not integers. In order to offset that, and limit it to integers, we also provide the "decimals" *facetType* to insist on having no numbers after the decimal point.

## Notes

As hinted at above, to the best of my knowledge, no implementation of the SDMX standard actually uses multiple Facets. Instead, they use one single Facet (often referred to as a TextFormat or a TextType), with each value of the FacetType enumeration becoming an attribute on the Facet. This has two advantages I can think of immediately, which is that you aren't repeating *facetValueType* a bunch and you can insist on the correct type for each FacetType. Let's look at the last example above, redone in this manner<sup>1</sup>:
```javascript
{
    "facetValueType": "exclusiveValueRange",
    "minValue": -6,
    "maxValue": 103,
    "decimals": 0
}
```
As you can see, we only needed one object to do the job that previously took three, and we could use numbers for -6, 103 and 0 instead of strings (because all three of *minValue*, *maxValue* and *decimals* always have to be numbers).

<sup>1</sup> - Note that this is a made up format to demonstrate how the idea might work. Here's an example ripped straight from the proposed SDMX-JSON standard:
```javascript
{
    "textType": "String",
    "maxLength": 1050
}
```