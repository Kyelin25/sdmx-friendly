# ItemScheme
[Information Model Description](../../information_model/Base/ItemScheme.md)

## Description

The ItemScheme is essentially just a list of things. The things themselves can contain things, giving you an implicit hierarchy of parent-child relationships between the things. Also, the things are nameable, meaning you can give them multi-lingual names and optionally descriptions.

That's pretty much it. As a base, abstract artefact, the ItemScheme itself just exists to provide this structure to be used by its child artefacts, and to allow other artefacts to refer to it in lieu of any of its more concrete children. For example, you might want to say "I'm happy to refer to any list of things", so you can just say "I'm happy to refer to any ItemScheme". An example of this is a Dimension, which can refer to any list of things (technically, though pretty rarely in practice).