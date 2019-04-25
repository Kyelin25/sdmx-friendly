
# ActionType





## Description

Used to specify the action that a receiving system should take when processing the content that is the object of the action.


## Values

**delete** (*string*): Data/Metadata is to be deleted.

**replace** (*string*): Data/Metadata is to be replaced, and may also include additional data/metadata to be appended.

**append** (*string*): Data or metadata is an incremental update for an existing data/metadata set or the provision of new data or documentation (attribute values) formerly absent. If any of the supplied data or metadata is already present, it will not replace that data or metadata. This corresponds to the "Update" value found in version 1.0 of the SDMX Technical Standards.

**information** (*string*): Data and metadata are for information purposes.


