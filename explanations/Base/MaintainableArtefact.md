# MaintainableArtefact
[Information Model Description](../../information_model/Base/MaintainableArtefact.md)

## Description

MaintainableArtefacts are all SDMX structures that need to be "maintained" by some organisation. This is a fairly fundamental concept in the SDMX Information Model; the idea that things like Codelists and DataStructureDefinitions should have somebody (specifically an Agency) in charge of them. This maintaining Agency has the responsibility of keeping its MaintainableArtefacts up-to-date by altering them if necessary. They're also who you can contact if you have questions about say, a DataStructureDefinition, or want them to add a Code to a Codelist.

To enable this, MaintainableArtefacts have an *id* (from IdentifiableArtefact) so that they can be identified, a reference to an Agency who is responsible for maintaining it and a *version* (from VersionableArtefact) to allow the versioning of changes. Versioning of changes is a pain, but is important so that people referring to the MaintainableArtefact know what they're getting, and when what they're getting has changed. For example, if a Code is deleted from a Codelist you're using in your data, you'd want to know.

Allegedly to make versioning easier, the *final* flag on MaintainableArtefacts lets you make changes without incrementing the *version*, as long as it's set to "false". However, in most implementations I've seen of SDMX, you're not allowed to refer to a non-final structure (as in using a non-final Codelist for a Dimension), even if you're doing so from **another** non-final structure, limiting its usefulness to playing about within the context of one single MaintainableArtefact.

The combination of the artefact type, the maintenance Agency, the *id* and the *version* is enough to uniquely identify any MaintainableArtefact, and this is then used to make it possible to identify **any** IdentifiableArtefact. See the explanation of [IdentifiableArtefact](IdentifiableArtefact.md) for details on how precisely this works.