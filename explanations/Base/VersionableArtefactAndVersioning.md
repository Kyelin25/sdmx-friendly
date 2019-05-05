# VersionableArtefact
[Definition](../../information_model/Base/VersionableArtefact.md)

## Description

Inheriting from VersionableArtefact gives you access to *version*, *validFrom* and *validTo*. I'm yet to see the *validFrom* and *validTo* fields be used, but in principle you can mark an object with them to make sure people and systems know when your object is valid. The *real* star of the show, though, is the *version*. This lets people and systems know when your objects change, and it's **required** as part of identifying objects (see [IdentifiableArtefact](IdentifiableArtefact.md) explanation for more detail).

As near as I can tell, there are no restrictions placed on the format of the *version* in the actual Information Model, but I believe every implementation requires it to be a series of .-separated numbers like (e.g. 1.0, 1.0.3, 1.0.4.11 and so on). I personally recommend using the Semantic Versioning system for deciding what *versions* to use (just Google it... it's very widely used). 

Because you need to use *version* to identify any object, when one object refers to another (for example, using a Codelist for a Dimension in a DataStructureDefinition, or even a single Concept), updating the *version* of a widely-used object can have very unpleasant flow-on updates (assuming you want things to continue using the latest version). Most implementations of SDMX will only let you make very limited changes to an object before requiring a version increment.

## Examples

Let's look at an example of what I'm going to call the Version Tsunami. You have a Codelist of countries. You set up your initial version and call it "1.0.0". You use it as the *coreRepresentation* for 5 separate Concepts (things like "Country of Birth", "Country of Origin", "Destination Country" etc). You also explicitly use it for a Dimension in a DataStructureDefinition. That DataStructureDefinition in turn is used by 6 DataflowDefinitions.

A new country comes into being, and now you need to add a Code to your Codelist. This change requires a version-change, so you increment it to 1.1.0, to let people know about the change. But now, because you want everything to keep using the most up to date version of your Codelist you have to update (and increment the version of) 5 Concepts, 1 DataStructureDefinition and 6 Dataflows. You added a Code to one Codelist and had to increment the version number of 13 objects.


## Notes

There's not a great way to get around the Version Tsunami with the way things are defined in the Information Model and Registry Specification. One possibility would be to go "all in" on the Semantic Versioning system, and allow objects to refer to other objects using version ranges. For example, a DataStructureDefinition when referring to a Codelist that's currently in version "1.0.1" could state (using some standardised notation) that it's happy to accept any version **after** "1.0.0" but before "2.0.0". As long as no breaking change was made to the Codelist (which would necessitate going to "2.0.0"), the DSD would just automatically receive the newest Codelist version.