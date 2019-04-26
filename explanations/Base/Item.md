# Item
[Information Model Description](../../information_model/Base/Item.md)

## Description

If an [ItemScheme](ItemScheme.md) is essentially just a list of things, then the Item is essentially just a thing. The thing has an identifier, a multi-lingual name (no, you don't need to provide anything other than your favourite language) and optionally a multi-lingual description. It also can have child items (this is how the ItemScheme can have an implicit hierarchy).

As an abstract artefact, the Item exists to provide a pattern for concrete artefacts like Codes and Categories to follow.

## Example

Let's build up a simple inheritance tree from a single person. Our inheritance tree represents the flow of inheritance from a wealthy family matriarch, Jenny. 

Because Item is abstract, for our example we're going to use the made-up artefact Person, which inherits everything from Item and doesn't add anything.

- **Id**: JNY **Name**: Jenny **Description**: Jenny is the first person in the tree, and the mother of this line of inheritance.
    - **Id**: BRY **Name**: Barry
        - **Id**: SRH **Name**: Sarah **Description**: Sarah is Jenny's favourite granddaughter
    - **Id**: JON **Name**: Jon **Description**: Jon offended Jenny at a recent luncheon and will receive only a lump of coal.
    - **Id**: EDT **Name**: Edith **Description**: Edith thinks she's receiving the house in Budapest, but will actually inherit Jenny's collection of ceramic cats.
        - **Id**: APL **Name**: Apple **Description**: Jenny disapproves of Apple's name. This is why Edith will only be inheriting the cats.
        - **Id**: BRY2 **Name**: Barry

In this set of Items, the parent-child relationship literally represents a parent-child relationship, and the flow of inheritance from the family's wealthy matriarch, Jenny. Note that although Edith named her son Barry after his uncle, we had to give him a different id to the "original" Barry, as the identifiers must be unique within the tree (actually unique within their parent ItemScheme).

## Notes

Artefacts that inherit from Item inherit the parent-child relationship, but flavour it so it can only refer to artefacts of the same type. That is, a Code can only have Codes as children, not any Item.

As an IdentifiableArtefact (inherited through NameableArtefact), an Item can only be referenced **through** its parent ItemScheme. In order to do this, each Item in an ItemScheme must have a unique identifier.