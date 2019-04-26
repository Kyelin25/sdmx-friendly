
# IdentifiableArtefactRef

Inherits from: [MaintainableArtefactRef](MaintainableArtefactRef.md)



## Description

Identification of the target object by means of its identifier constructs i.e. agency ID, id, version and the IdentifiableObject id.


## Attributes

### Inherited

**agencyID** (*string*): The AgencyID of the referenced object.

**id** (*string*): The id of the referenced object.

**version** (*string*): The version of the referenced object.



## References

**containedObject** ([IdentifiableArtefactRef](IdentifiableArtefactRef.md) - 0..1): Association to a contained object in a hierarchy of IdentifiableArtefacts, such as a Transition in a ProcessStep.

### Inherited



## Referenced By

[IdentifiableArtefactRef](IdentifiableArtefactRef.md) (as containedObject)


