# Item
[Definition](../../information_model/Base/Item.md)

## Description

If an [ItemScheme](ItemScheme.md) is essentially just a list of things, then the Item is essentially just a thing. The thing has an identifier, a multi-lingual name (no, you don't need to provide anything other than your favourite language) and optionally a multi-lingual description. It also can have child items (this is how the ItemScheme can have an implicit hierarchy).

As an abstract artefact, the Item exists to provide a pattern for concrete artefacts like Codes and Categories to follow.

## Examples

Let's build up a simple inheritance tree from a single person. Our inheritance tree represents the flow of inheritance from a wealthy family matriarch, Jenny. 

Because Item is abstract, for our example we're going to use the made-up artefact Person, which inherits everything from Item and doesn't add anything.

```javascript
{
    "id": "JNY",
    "name": [{"en", "Jenny"}]
    "description": [{"en", "Jenny is the first person in the tree, and the mother of this line of inheritance."}],
    "items":[
        {
            "id": "BRY",
            "name": [{"en", "Barry"}]
            "items":[
                {
                    "id": "SRH",
                    "name": [{"en", "Sarah"}],
                    "description": [{"en", "Sarah is Jenny's favourite granddaughter."}]
                }
            ]
        },
        {
            "id": "JON",
            "name": [{"en", "Jon"}],
            "description": [{"en", "Jon offended Jenny at a recent luncheon and will receive only a lump of coal."}]
        },
        {
            "id": "EDT",
            "name": [{"en", "Edith"}],
            "description": [{"en", "Edith thinks she's receiving the house in Budapest, but will actually inherit Jenny's collection of ceramic cats."}],
            "items": [
                {
                    "id": "APL",
                    "name": [{"en", "Apple"}],
                    "description": [{"en", "Jenny disapproves of Apple's name. This is why Edith will only be inheriting the cats."}]
                },
                {
                    "id": "BRY",
                    "name": [{"en", "Barry"}]
                }
            ]
        }
    ]
}
```

In this set of Items, the parent-child relationship literally represents a parent-child relationship, and the flow of inheritance from the family's wealthy matriarch, Jenny. Note that although Edith named her son Barry after his uncle, we didn't have to give him a different id, as he falls under a different parent in the tree. It's important to note that this is not true for all concrete implementations of Item (see Code for one where this is not true), and I'll specify in each of them which is the case.

If we assume that these Persons live inside a PersonScheme with AgencyId *SDMX*, Id *PS_JNY_MONEY* and Version *1.0.2* (see explanation of [MaintainableArtefact](MaintainableArtefact.md) for why we need to know this), we can uniquely refer to any Person in this scheme using that plus the chain of Person ids to them. For example, say we want to refer to Edith's son Barry: SDMX:PS_JNY_MONEY(1.0.2).JNY.EDT.BRY is enough to uniquely identify him.

## Notes

Artefacts that inherit from Item inherit the parent-child relationship, but flavour it so it can only refer to artefacts of the same type. That is, a Code can only have Codes as children, not any Item.

As an IdentifiableArtefact (inherited through NameableArtefact), an Item can only be referenced **through** its parent ItemScheme. In order to do this, each Item in an ItemScheme must have a unique identifier **to some degree** (i.e. unique within its ItemScheme vs unique amongst its siblings). Unfortunately, which is the case depends on the concrete implementations of ItemScheme and Item (just to confuse you). I will explain in each one specifically how to identify an individual Item.