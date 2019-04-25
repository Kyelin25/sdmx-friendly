
# ComponentMap

Inherits from: [AnnotableArtefact](../Base/AnnotableArtefact.md)



## Description

Links a source and target Component where there is a semantic equivalence between the source and target Components.


## Attributes

alias: string

preferredLanguage: string



## References

source: [Component](../Base/Component.md) (One) - Association to the source Component.

target: [Component](../Base/Component.md) (One) - Association to the target Component.

contentMap: [RepresentationMapping](RepresentationMapping.md) (ZeroOrOne) - Association to the constructs that map the content of the Components - this will be either one of the subclasses of ItemScheme or a mapping to text.

contains: [Annotation](../Base/Annotation.md) (ZeroOrMany) - No description



## Referenced By

[StructureMap](StructureMap.md) (as map)


