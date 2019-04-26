# Item
[Information Model Description](../../information_model/Base/IdentifiableArtefact.md)

## Description

IdentifiableArtefact is the base abstract class that allows inheriting classes to be identified (hence the name). This is done using the *id* and *urn* fields. It's worth noting that although the Information Model says that *id* is the "unique identifier of the object*, this doesn't appear to be globally unique. It must be unique as an IdentifiableArtefact contained inside a MaintainableArtefact, but otherwise I think it's pretty open slather. 

In order to globally uniquely identify an IdentifiableArtefact, you need to use the *urn*. Although the Information Model doesn't specify how this should be structured, the Registry Specification does. It must be structured so:
```
urn:sdmx:org.sdmx.infomodel{structureType}={AgencyId}:{Id}({Version}){IdChain}
```
Let's break down what each of these components mean, then show some examples.
- **structureType**: What SDMX structure we're referring to, in the following format: urn:sdmx:org.sdmx.infomodel.