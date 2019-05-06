# ConceptScheme and Concept
[ConceptScheme Definition](../../information_model/ConceptScheme/ConceptScheme.md) [Concept Definition](../../information_model/ConceptScheme/Concept.md)

## Description

The Concept is one of the most fundamental (and in my opinion confusing) parts of the SDMX standard. Whenever I try describe what a Concept is I end up using words like "thing", "concept, but with a small c" and "idea". Concepts exist in SDMX to give **meaning** to other things. By reusing them, you can encode the idea (dammit) that certain objects have semantic equivalence. For example, if two Dimensions in two different DataStructureDefinitions both take meaning from the same Concept, it's not insane to think they are equivalent in some way.

Concepts are maintained in ConceptSchemes, where their parent-child hierarchy (inherited from Item) can show semantic links between Concepts. For example, you might have the following parent-child chain of Concepts.
- Country
    - Country of Birth
        - Country of Birth of Person
        - Country of Birth of Mother
        - Country of Birth of Father

You can see how 