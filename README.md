# ReadAloud dictionaries

Offline word meanings for [ReadAloud Studio](https://github.com/zezetata), an app for learning English:
one small SQLite file per language, holding the meanings of the most common English words in that
language. The app downloads the one for the learner's language and shows a word's meaning with no
connection.

## Packs

Release **packs-2026-10**, made from the translation tables of English Wiktionary as extracted on
3 October 2026. For each of the 42,044 most common English words in their dictionary form, a pack has
up to four translations per part of speech, one sense at a time, with archaic, rare, crude and sexual
senses left out.

| File | Language | Words |
| --- | --- | --- |
| meanings-es.sqlite | Spanish | 25,204 |
| meanings-fr.sqlite | French | 24,856 |
| meanings-de.sqlite | German | 24,841 |
| meanings-ru.sqlite | Russian | 23,312 |
| meanings-pl.sqlite | Polish | 22,518 |
| meanings-pt.sqlite | Portuguese | 21,965 |
| meanings-it.sqlite | Italian | 20,980 |
| meanings-nl.sqlite | Dutch | 18,581 |
| meanings-ja.sqlite | Japanese | 15,395 |
| meanings-tr.sqlite | Turkish | 13,397 |
| meanings-uk.sqlite | Ukrainian | 13,004 |
| meanings-ar.sqlite | Arabic | 11,277 |
| meanings-ko.sqlite | Korean | 11,239 |
| meanings-hi.sqlite | Hindi | 8,903 |
| meanings-vi.sqlite | Vietnamese | 8,546 |
| meanings-id.sqlite | Indonesian | 8,523 |
| meanings-fa.sqlite | Persian | 7,132 |
| meanings-th.sqlite | Thai | 7,085 |
| meanings-ms.sqlite | Malay | 6,782 |

## Format

Each file has two tables. `meta(key, value)` holds `schema` (1), `language` and `source`.
`meanings(word, meaning)` holds a word in lower case and its meaning, one line per part of speech:

```
run   v. correr; dirigir; funcionar
      n. carrera; partida; temporada
```

## Credit and licence

The translations are the work of the contributors to [English Wiktionary](https://en.wiktionary.org),
extracted by [Wiktextract](https://github.com/tatuylonen/wiktextract) and published at
[kaikki.org](https://kaikki.org). Wiktionary's text is licensed under the
[Creative Commons Attribution-ShareAlike 4.0 International licence](https://creativecommons.org/licenses/by-sa/4.0/)
(and the GFDL). These packs adapt it (selection, ordering and formatting), and are shared under the
same licence: CC BY-SA 4.0. See LICENSE.
