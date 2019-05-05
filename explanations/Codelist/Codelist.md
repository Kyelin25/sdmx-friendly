# Codelist and Code
[Codelist Definition](../../information_model/Codelist/Codelist.md) [Code Definition](../../information_model/Codelist/Code.md)

## Description

A Codelist is a specific instance of ItemScheme, used to provide a list of values. Essentially it's what you're going to be using most of the time for a Dimension, to show which values it can take. Think a list of all countries in the world, with each country being represented by a Code. Each Code gets a multi-lingual *name* and (optionally) *description*. The *id* inherited from IdentifiableArtefact should ideally be something semi-descriptive, rather than just a number or random text string, as it'll be used in API calls to query data, and the names don't come down with the data (so you'll get "AUS" in the data message instead of "Australia").

You can use the parent-child relationships inherited from Item to construct a simple hierarchy. I **do** mean simple, though. Each Code can only have one parent, and there are no explicit levels (like there are in many statistical classifications). Any "levels" are merely implicit. For example, the "third" level would be the Codes you have to go through two other parent Codes to reach. If you want to model a more complex hierarchy, you should use a [HierarchicalCodelist](../../information_model/Codelist/HierarchichalCodelist.md).

## Best Practice

- Prepend "CL_" to the beginning of Codelist ids, so it's clear if anybody sees it on its own that it refers to a Codelist
- Code ids should be semi-descriptive and in all capitals
- Reuse existing Codelists where possible. Check the [Global SDMX Registry](https://registry.sdmx.org) to see if there is already a globally-recognized Codelist that does what you want

## Examples

For a table with Australian State or Territory of Residence for one of the Dimensions, you might use the following Codelist as its representation:
```javascript
{
    "id": "CL_AUS_STATES", // Note the CL_ prefix to denote a Codelist
    "agencyId": "ABS",
    "version": "1.0.0",
    "name":[
        {"en", "Australian States"}
    ],
    "codes":[
        {
            "id": "AUS",
            "name":[
                {"en", "Australia"}
            ],
            "codes":[
                {
                    "id": "NSW",
                    "name": [
                        {"en", "New South Wales"}
                    ]
                },
                {
                    "id": "VIC",
                    "name": [
                        {"en", "Victoria"}
                    ]
                },
                {
                    "id": "QLD",
                    "name": [
                        {"en", "Queensland"}
                    ]
                },
                {
                    "id": "SA",
                    "name": [
                        {"en", "South Australia"}
                    ]
                },
                {
                    "id": "WA",
                    "name": [
                        {"en", "Western Australia"}
                    ]
                },
                {
                    "id": "TAS",
                    "name": [
                        {"en", "Tasmania"}
                    ]
                },
                {
                    "id": "NT",
                    "name": [
                        {"en", "Northern Territory"}
                    ]
                },
                {
                    "id": "ACT",
                    "name": [
                        {"en", "Australian Capital Territory"}
                    ]
                }
            ]
        }
    ]
}
```

## Notes

Although Codes have parents, and are maintained in a hierarchy, they're not stored that way. This means that Code *ids* need to be unique within their Codelist. Contrast this to Categories (another instance of Item/ItemScheme), which are stored in their hierarchy and can share *ids*. This makes sense if you consider that you need to be able to use a single id to refer to one Code when doing data queries.

## Identification

Identification of a Codelist works just like any other MaintainableArtefact (see [IdentifiableArtefact](../Base/IdentifiableArtefact.md) for details).

As mentioned in the Notes section, Codes are not stored in hierarchy. This means a Code's parent codes are ignored when identifying it as per the rules laid out in the [IdentifiableArtefact](../Base/IdentifiableArtefact.md) explanation. So a Code is always identified like so:
```
    urn:sdmx:org.sdmx.infomodel.codelist.Code={AgencyIdChain}:{CodelistId}({CodelistVersion}).{CodeId}
```

For example, identifying the ACT (a child Code of AUS) in the Codelist used in the Examples section would look like:
```
    urn:sdmx:org.sdmx.infomodel.codelist.Code=ABS:CL_AUS_STATES(1.0.0).ACT
```