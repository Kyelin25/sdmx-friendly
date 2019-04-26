# AnnotableArtefact and Annotation
[AnnotableArtefact Information Model Description](../../information_model/Base/AnnotableArtefact.md) [Annotation Information Model Description](../../information_model/Base/Annotation.md)

## Description

The AnnotableArtefact is not the most fascinating SDMX artefact, so I've bundled it with the Annotation, as that's where all the action is. As an abstract artefact, the AnnotableArtefact just provides the ability for other artefacts to have Annotations attached.

What are Annotations? Essentially, whatever you want them to be. They can be used to add extra descriptive information to an artefact (like attaching a note to a DataStructureDefinition saying: "This was designed by committee and so doesn't really satisfy anybody") or even as semi-extensions to the SDMX standard to change the behaviour of consuming systems (like providing alternate labels for a Code, or specifying that a Dimension should not be displayed on screen, as it only has one value).

When creating an Annotation, you can provide an *id*, a *title*, a *type*, a *url* and some multi-lingual *text*. Despite having an *id*, Annotation doesn't inherit from IdentifiableArtefact, and so this is not required. In fact, as near as I can tell, none of these are actually required, though it's probably a good idea to provide a *type*, so that people (or systems) know how to interpret the Annotation.

## Examples

Let's put together a few examples of Annotations. The first is meant to be read by humans, and provides further information about a Codelist. For anybody who actually understands French, I am **so** sorry for the terrible translation.
```javascript
{
    "type":"CONSTRUCTOR_COMMENT",
    "text":
    {
        "en": "This Codelist is the combination of two statistical classifications for display purposes, and should not be taken as a statistical classification in its own right.",
        "fr": "Cette liste de codes est la combinaison de deux classifications statistiques aux fins d'affichage et ne doit pas être considérée comme une classification statistique à part entière."
    }
}
```

We can see here we've used the *type*, to help people understand that this is a comment from the constructor of the Codelist, and the *text*, in order to provide a multi-lingual comment. Clearly this is intended to be read by a human, however there's nothing stopping a system from using it. For example, perhaps all *CONSTRUCTOR_COMMENT* Annotations should be displayed as little pop-ups over the Codelist.

The second example would be attached to a DataflowDefinition to tell a presentation system to hide the specified Dimensions (as in this Dataflow we've constrained them to only one value, and don't actually want them seen).
```javascript
{
    "type": "HIDDEN",
    "title": "AGE"
}
```

Here we've used the *type* again, which is necessary for the presentation system to know what to do with this Annotation. We're using *title* to provide the id of the Dimension to hide. Using *text* for this purpose would be ridiculous, as the Dimension has the same id in every language.

Finally, let's look at perhaps a bit of a stretched example. We want to attach an Annotation to each Code in a Codelist that represents the countries of the world. The Annotation is to be used by a presentation system to retrieve and display each country's flag.
```javascript
{
    "type": "FLAG_LINK",
    "url": "https://flagsoftheworld.org/Australia/100_200.jpg"
}
```

Here in addition to the *type* field, we add a use of the *url* field to specify the location to go to in order to retrieve (in this case) Australia's flag.