# CategoryScheme, Category and Categorisation
[CategoryScheme Definition](../../information_model/CategoryScheme/CategoryScheme.md) [Category Definition](../../information_model/CategoryScheme/Category.md) [Categorisation Definition](../../information_model/CategoryScheme/Categorisation.md)

## Description

The CategoryScheme (a subclass of ItemScheme) is used to categorize artefacts. That is, it lets you apply some sort of taxonomy to artefacts, generally for the purpose of discoverability. The CategoryScheme and Category defines this taxonomy, and then Categorisations link artefacts (any IdentifiableArtefact is fair game, but you're most likely to use DataflowDefinitions and DataStructureDefinitions). It's important to note that any number of artefacts can be categorised into any number of Categories. Importantly this means each artefact isn't limited to belonging to only one Category (though you may want to do so to avoid confusion).

The canonical example of this is if you have a set of topics you release statistics under. You know, the usual: Economics, Environment, Agricultural and whatnot. You design a CategoryScheme that contains Categories for each topic you release data for (using the parent-child hierarchy Category inherits from Item to give the topic-tree structure), and then you can use Categorisations to link each Dataflow and DSD to any number of appropriate Categories. This then would allow users to "explore" your statistics by selecting topics. Doing so would then expose all Dataflows and DSDs that are Categorised to the selected topic (Category).

Another use-case makes use of the fact that any IdentifiableArtefact can be referred to be a Categorisation. If your organisation maintains official statistical classifications (either as Codelists or HierarchicalCodelists), these two could be classified into the topics to which they belong.

As CategoryScheme and Category both are subclasses of NameableArtefact (via ItemScheme and Item respectively), you must provide a *name* for them (why wouldn't you!) and can optionally provide a *description* also. You can imagine that the name would provide the text of a topic that the user could click on, and the description might be available as a pop-up or pop-under to describe the topic to the user.

## Best Practice

- Category ids should be semi-descriptive and in all capitals


## Example

```javascript
{
    "id": "TOPICS",
    "agencyId": "ABS",
    "version": "1.0.0",
    "name": [{"en", "ABS Topics Framework"}],
    "categories":[
        {
            "id": "ECONOMY",
            "name": [{"en", "Economic Statistics"}],
            "categories":[
                {
                    "id": "BUS_IND",
                    "name": [{"en", "Business Indicators"}]
                },
                {
                    "id": "FINANCE",
                    "name": [{"en", "Finance"}]
                }
            ]
        },
        {
            "id": "INDUSTRY",
            "name": [{"en", "Industrial Statistics"}]
            "categories":[
                {
                    "id": "AGRICULTURE",
                    "name": [{"en", "Agricultural Statistics"}]
                },
                {
                    "id": "RT",
                    "name": [{"en", "Retail and Wholesale Trade Statistics"}]
                }
            ]
        }
    ]
}
```

Here we have duplicated a (very) pared-down version of the Topics framework currently in use (2019-05) on the Australian Bureau of Statistics website. This could then be used to categorise all statistical releases. The list of Topics could be displayed on the front page of your organisation's website, and users could click through the Categories to find statistics that most interest them.

## Notes

Categories are stored hierarchically (contrasted with Codes). This means that unlike Codes, the *id* of a Category does not need to be unique within its CategoryScheme, only unique within its siblings. That is, Categories that share a parent Category must have different *ids* (this applies to the top-level Categories as well). Otherwise, it's open slather. This permitted duplication of *ids* can be seen in the identification paradigm below.

We've focussed on the idea of a Topics framework, as the most likely use of Categories, but it's important to remember that Categories are a very abstract tool, and could be used for any taxonomy purposes. For example, perhaps you could have a CategoryScheme used to classify statistics by which groups of people would most find them interesting, or by ongoing vs one-off status.

## Identification

Identification of a CategoryScheme or Categorisation works just like any other MaintainableArtefact (see [IdentifiableArtefact](../Base/IdentifiableArtefact.md) for details).

As mentioned in the Notes, Categories are stored hierarchically, so a Category's ancestors must be taken into account when identifying it. So a Category is always identified like so:
```
    urn:sdmx:org.sdmx.infomodel.categoryscheme.Category={AgencyIdChain}:{CategorySchemeId}({CategorySchemeVersion}).{AncestorCategoryIdChain}.{CategoryId}
```

 For example, in the CategoryScheme example used in the Examples section, we would identify the Busines Indicators Category using its containing Category:
 ```
    urn:sdmx:org.sdmx.infomodel.categoryscheme.Category=ABS:TOPICS(1.0.0).ECONOMY.BUS_IND
 ```