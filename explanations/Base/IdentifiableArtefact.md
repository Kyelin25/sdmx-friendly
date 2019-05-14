# IdentifiableArtefact
[Definition](../../information_model/Base/IdentifiableArtefact.md)

## Description

IdentifiableArtefact is the base abstract class that allows inheriting classes to be identified (hence the name). This is done using the *id* and *urn* fields. It's worth noting that although the Information Model says that *id* is the "unique identifier of the object*, this doesn't appear to be globally unique.

IdentifiableArtefacts need to be either also a MaintainableArtefact (more specific than just being Identifiable), or contained within a MaintainableArtefact. For example, a Codelist is a MaintainableArtefact so is fine. A Code is not a MaintainableArtefact, but it **is** contained inside a MaintainableArtefact; the Codelist. Why this is required will become apparent when looking at how to use the *urn* to globally uniquely identify an object.

In order to globally uniquely identify an IdentifiableArtefact, you need to use the *urn*. Although the Information Model doesn't specify how this should be structured, the Registry Specification does. It must be structured like so:
```
urn:sdmx:org.sdmx.infomodel.{packageName}.{structureType}={AgencyIdChain}:{MaintainableId}({Version}){IdChain}
```
Let's break down what each of these components mean, then show some examples.
- **packageName**: Which SDMX Information Model package our *structureType* belongs to. For example, Code belongs in the "codelist" package. The packages are how we've structured this repository.
- **structureType**: The type of SDMX structure we're referring to. For example, Codelist or DataStructureDefinition.
- **AgencyIdChain**: The chain of maintenance Agencies responsible for maintaining either the object we're referring to, or its parent MaintainableArtefact if it's not Maintainable itself. For example, IMF.FIN or merely IMF. See the explanation of [Agencies](AgencySchemeAndAgencies.md) for more detail about Agency chaining.
- **MaintainableId**: This is either the *id* of the object if it's a MaintainableArtefact, or the *id* of its parent MaintainableArtefact if it is not.
- **Version**: This is either the *version* of the object if it's a MaintainableArtefact, or the *version* of its parent MaintainableArtefact if it is not.
- **IdChain**: In the case of a MaintainableArtefact, this is not specified, as the previous elements are enough to uniquely identify it. When talking about a non-Maintainable object (e.g. a Code in a Codelist or a MetadataAttribute in a ReportStructure in a MetadataStructureDefinition), this will contain a .-delimited list of identifiers (traversing a series of containing objects) that terminates in the *id* of the object we're referring to. If there is no maintained hierarchy of containers (this varies based on the artefact), this will be one single *id*. Note that even if there is a containing object, if there is only ever one (for example, a DimensionDescriptor in a DataStructureDefinition) it's omitted from the IdChain.

## Examples

Referring to *version* "1.0.2" of a Codelist, maintained by the IMF directly, with the *id* "CL_AGE":
```
    urn:sdmx:org.sdmx.infomodel.codelist.Codelist=IMF:CL_AGE(1.0.2)
```
Here we see that no *IdChain* was necessary, as Codelists are Maintainable, and the *AgencyIdChain* consisted of only one agency.

Referring to a top-level Code with id "Y0T4" in the previously-used Codelist (CL_AGE):
```
    urn:sdmx:org.sdmx.infomodel.codelist.Code=IMF:CL_AGE(1.0.2).Y0T4
```
This is very similar to the previous example. We change the "Codelist" *structureType* to "Code", to indicate what we're looking for, and add a single *id* to the end.

Referring to a Category with id "LF", itself a child Category for a Category with id "ECO", all contained in version "2.1.0" of CategoryScheme maintained directly by the IMF, with *id* "CATS_TOPICS":
```
    urn:sdmx:org.sdmx.infomodel.categoryscheme.Category=IMF:CATS_TOPICS(2.1.0).ECO.LF
```
Of particular note in this example is that our *IdChain* now has two *ids* in it, as "LF" is a child Category of "ECO", so we need to go through "ECO" to get to "LF".


Referring to a Code with id "Y1", a child of the previously-used Code (Y0T4):
```
    urn:sdmx:org.sdmx.infomodel.codelist.Code=IMF:CL_AGE(1.0.2).Y1
```
I fooled you with that one, didn't I? Did you expect there to an *IdChain* of "Y0T4.Y1"? Yeah, I did too. Apparently, because Codelist Codes are not maintained in a hierarchy (I couldn't find where this was explicitly stated in the Information Model), despite **having** a hierarchy, you just refer directly to the Code of interest, thus having a single entry in the *IdChain*.