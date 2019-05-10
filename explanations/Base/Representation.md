# Representation
[Description](../../information_model/Base/Representation.md)

## Description

A Representation in SDMX is the answer to the question "What values can I take?" Generally when you're defining things in structural metadata that constrain values, they'll have a Representation. The most obvious example is a Dimension in a DataStructureDefinition. The Representation here defines what values reported observations can take for that Dimension. In the case of a [MetadataAttribute](../../MetadataStructure/MetadataAttribute.md), it defines what values that attribute can take in provided reports. Seeing a pattern? For a full list of artefacts that can have a Representation, take a look at the [Information Model Description](../../information_model/Base/Representation.md#Referenced%20By).

There are two types of Representation: enumerated and non-enumerated.

### Enumerated Representations

An enumerated Representation takes its acceptable values from the *ids* of an ItemScheme. To be clear, it provides a reference to a concrete subclass of ItemScheme (like Codelist or CategoryScheme), and the valid values of whatever is **using** the Representation become whatever *ids* the items in the ItemScheme provide. In most cases, the Representation used by a Dimension will be of this type. This provides right off the bat a finite set of acceptable values for the Dimension.

To make things more complicated, although in general an enumerated Representation may refer to any ItemScheme, in practice, for a lot of artefacts the allowable target ItemScheme is constrained to only a few subclasses. An example might be the best way to explain this. Dimensions (in a DataStructureDefinition) that use an enumerated Representation must refer to a Codelist. The restrictions on Representations will be stated in the explanation of each Representation-using artefact, but I'll list them in the Notes section of this page as well for reference.

In addition to referring to an ItemScheme, an enumerated Representation may provide an *enumerationFormat*. This is something I have yet to work out the purpose for. In terms of definition, it is defined using [Facets](../Base/Facets.md) (but should only use Facets that are valid for *ids*). I believe it's supposed to provide some information about what textual format the *ids* of the target ItemScheme are in (like, are they all alphanumeric, or just alpha, or all three letters long, etc), and it doesn't seem to actually constrain values. As far as I can see, it doesn't really seem to be used.

As previously mentioned, Dimensions are most commonly going to have enumerated Representations. In fact, most DataAttributes will probably be enumerated as well.

### Non-Enumerated Representations

A non-enumerated Representation determines its acceptable values by providing a number of Facets which constrain them. See the explanation of [Facets](../Base/Facets.md) for precisely how this works. Non-enumerated Representations don't rely on a pre-defined set of allowable values like enumerated Representations do. In fact, their allowable values can be infinite. The TimeDimension in a DataStructureDefinition always has a non-enumerated Representation. This makes sense, as it's impossible to list in advance every single possible time value (even if you're constrained to just years!).

Another common use of the non-enumerated Representation is to allow a "comments" DataAttribute, which takes any textual comment.