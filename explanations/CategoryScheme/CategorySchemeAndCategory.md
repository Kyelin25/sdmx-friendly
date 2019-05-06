# CategoryScheme, Category and Categorisation
[CategoryScheme Definition](../../information_model/CategoryScheme/CategoryScheme.md) [Category Definition](../../information_model/CategoryScheme/Category.md) [Categorisation Definition](../../information_model/CategoryScheme/Categorisation.md)

## Description

The CategoryScheme (a subclass of ItemScheme) is used to categorize artefacts. That is, it lets you apply some sort of taxonomy to artefacts, generally for the purpose of discoverability. The CategoryScheme and Category defines this taxonomy, and then Categorisations link artefacts (any IdentifiableArtefact is fair game, but you're most likely to use DataflowDefinitions and DataStructureDefinitions).

The canonical example of this is if you have a set of topics you release statistics under. You know, the usual: Economics, Environment, Agricultural and whatnot. You design a CategoryScheme that contains Categories for each topic you release data for (using the parent-child hierarchy Category inherits from Item to give the topic-tree structure), and then you can use Categorisations to link each Dataflow and DSD to any number of appropriate Categories. This then would allow users to "explore" your statistics by selecting topics. Doing so would then expose all Dataflows and DSDs that are Categorised to the selected topic (Category).

As CategoryScheme and Category both are subclasses of NameableArtefact (via ItemScheme and Item respectively), you must provide a *name* for them (why wouldn't you!) and can optionally provide a *description* also. You can imagine that the name would provide the text of a topic that the user could click on, and the description might be available as a pop-up or pop-under to describe the topic to the user.

## Best Practice

- Category ids should be semi-descriptive and in all capitals


## Example

## Notes

Categories are stored hierarchically (contrasted with Codes). This means that unlike Codes, the *id* of a Category does not need to be unique within its CategoryScheme, only unique within its siblings. That is, Categories that share a parent Category must have different *ids* (this applies to the top-level Categories as well). Otherwise, it's open slather. This permitted duplication of *ids* can be seen in the identification paradigm below.

## Identification

Identification of a CategoryScheme or Categorisation works just like any other MaintainableArtefact (see [IdentifiableArtefact](../Base/IdentifiableArtefact.md) for details).

As mentioned in the Notes, Categories are stored hierarchically, so a Category's ancestors must be taken into account when identifying it. So a Category is always identified like so:
```
    urn:sdmx:org.sdmx.infomodel.categoryscheme.Category={AgencyIdChain}:{CategorySchemeId}({CategorySchemeVersion}).{AncestorCategoryIdChain}.{CategoryId}
```

 For example, in the CategoryScheme example used in the Examples section, we would identify the Labour Force Statistics Category using its containing Categories:
 ```
    urn:sdmx:org.sdmx.infomodel.categoryscheme.Category=ABS:CATS_TOPICS(1.0.2).ECO.LABOUR.LFS
 ```