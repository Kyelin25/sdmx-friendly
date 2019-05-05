# NameableArtefact
[Definition](../../information_model/Base/NameableArtefact.md)

## Description

The NameableArtefact needs very little description. Its use as a superclass is essentially just a way of saying "hey, you **must** give this thing a name, and you **can** give it a description if you want." Both the *name* and the *description* are InternationalStrings, so you can provide as many languages (in fact, locales, which is even better) as you want.

## Notes

It's worth noting that there's no way of requiring the *name* to have any given locale. For instance, you might require that all named objects have a Spanish and a German name, but there's no way in the model to do this (though you could use Annotations to help).

Unfortunately (or fortunately?) because NameableArtefact inherits from IdentifiableArtefact, there's no "nice" way to mark an artefact as needing a name but not be identifiable.