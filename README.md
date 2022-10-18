# dexie Community Translations

[dexie](https://dexie.space) should be accessible for all, and that includes languages. Everyone is invited to improve existing translations or create new ones.

## Participate
To participate, simply clone this repository, make the changes, and create a pull request. Alternatively, you can also edit the file directly on Github, without having to clone the repository first.

Each language has its own directory, containing a single translation.json, which is a JSON File containing all words of dexie. The left side (green text) contains the pointer and should not be changed, the right side (blue text) is the text displayed to the user, this is the translation that can be edited. Be careful to keep the quotes.

Example:
```json
"Connect Wallet": "지갑 연동",
```

## Plurals
Translation pointers which contain the `{{count}}` variable, may have additional sub-pointers for plurals (`_one`, `_other`, `_few`, `_many`), depending on the language. More about plurals here: https://www.i18next.com/translation-function/plurals

Example for English (one plural):
```json
{
  "You have {{count}} offers_one": "You have {{count}} offer",
  "You have {{count}} offers_other": "You have {{count}} offers",
}
```

Example for Polish (multiple plurals):
```json
{
  "You have {{count}} offers_one": "Masz {{count}} ofertę",
  "You have {{count}} offers_few": "Masz {{count}} oferty",
  "You have {{count}} offers_many": "Masz {{count}} ofert",
  "You have {{count}} offers_other": "Masz {{count}} ofert",
}
```

## New language
To add a new language, simply create a new directory and name it with the [ISO 639-1 code](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes) of your language. You can copy the JSON file from an existing language into the new directory as a template.

## Test Translations
All translations are automatically updated after merging on [dexie Testnet](https://testnet.dexie.space).

Translations will usually go live on Mainnet in the next weekly update.

## Questions?
Head over to our [dexie discord](https://discord.gg/3xUrkAxUmd) and join the channel #translators. If you are not familiar with Github, you can also submit translations or suggestions there.
