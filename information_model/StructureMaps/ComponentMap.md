
# ComponentMap

Inherits from: [AnnotableArtefact](../Base/AnnotableArtefact.md)



## Description

Links a source and target Component where there is a semantic equivalence between the source and target Components.


## Attributes

**alias** (*string*): An alternate identification of the map, that allows relation of multiple maps to be expressed by the sharing of this value.

**preferredLanguage** (*string*): Specifies the language to use for the content of the ToTextFormat option of RepresentationMap.

### Inherited



## References

### Inherited

**source** ([Component](../Base/Component.md) - 1): Association to the source Component.
**target** ([Component](../Base/Component.md) - 1): Association to the target Component.
**contentMap** ([RepresentationMapping](RepresentationMapping.md) - 0..1): Association to the constructs that map the content of the Components - this will be either one of the subclasses of ItemScheme or a mapping to text.
**contains** ([Annotation](../Base/Annotation.md) - 0..*): No description


## Referenced By

[StructureMap](StructureMap.md) (as map)


