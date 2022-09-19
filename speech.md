---
description: Use text-to-speech, speech-to-text, and translation functions in your app
---

# Speech

## Video Tutorial

You can see the [Text to Speech](speech.md#text-to-speech) and [Translation](speech.md#translation) blocks in use in this video tutorial:

{% embed url="https://www.youtube.com/watch?v=0NrkKiCGaxk" %}

## Text to Speech

Read a piece of text aloud in a specified language.

![](<.gitbook/assets/image (153).png>)

### Supported text to speech languages

| Language          | Android | iOS | Web |
| ----------------- | ------- | --- | --- |
| Afrikaans         | ✅       | ✅   | ✅   |
| Albanian          | ❌       | ✅   | ✅   |
| Arabic            | ✅       | ✅   | ✅   |
| Armenian          | ✅       | ❌   | ❌   |
| Azerbaijan        | ✅       | ✅   | ✅   |
| Basque            | ✅       | ✅   | ✅   |
| Belarusian        | ✅       | ❌   | ❌   |
| Bengali           | ✅       | ❌   | ❌   |
| Bosnian           | ❌       | ✅   | ✅   |
| Bulgarian         | ❌       | ✅   | ❌   |
| Catalan           | ✅       | ✅   | ✅   |
| Cebuano           | ✅       | ✅   | ✅   |
| Chinese China     | ✅       | ✅   | ✅   |
| Chinese Hong Kong | ✅       | ✅   | ✅   |
| Chinese Taiwan    | ✅       | ✅   | ✅   |
| Croatian          | ❌       | ✅   | ✅   |
| Czech             | ✅       | ✅   | ✅   |
| Danish            | ✅       | ✅   | ✅   |
| Dutch             | ✅       | ✅   | ✅   |
| English GB        | ✅       | ✅   | ✅   |
| English US        | ✅       | ✅   | ✅   |
| Esperanto         | ✅       | ✅   | ✅   |
| Estonian          | ✅       | ✅   | ✅   |
| Finnish           | ✅       | ✅   | ✅   |
| French            | ✅       | ✅   | ✅   |
| Galician          | ✅       | ✅   | ✅   |
| Georgian          | ✅       | ❌   | ❌   |
| German            | ✅       | ✅   | ✅   |
| Greek             | ✅       | ✅   | ✅   |
| Gujarati          | ✅       | ❌   | ❌   |
| Haitian Creole    | ✅       | ✅   | ✅   |
| Hebrew            | ✅       | ✅   | ✅   |
| Hill Mari         | ✅       | ✅   | ❌   |
| Hindi             | ✅       | ✅   | ✅   |
| Hungarian         | ✅       | ✅   | ✅   |
| Icelandic         | ✅       | ✅   | ✅   |
| Indonesian        | ✅       | ✅   | ✅   |
| Italian           | ✅       | ✅   | ✅   |
| Irish             | ✅       | ✅   | ✅   |
| Japanese          | ✅       | ✅   | ✅   |
| Javanese          | ✅       | ✅   | ✅   |
| Kannada           | ✅       | ❌   | ❌   |
| Kazakh            | ✅       | ✅   | ❌   |
| Khmer             | ✅       | ❌   | ❌   |
| Korean            | ✅       | ✅   | ✅   |
| Kyrgyz            | ❌       | ✅   | ❌   |
| Latin             | ❌       | ✅   | ✅   |
| Latvian           | ✅       | ✅   | ✅   |
| Lithuanian        | ✅       | ✅   | ✅   |
| Luxembourgish     | ✅       | ✅   | ✅   |
| Macedonian        | ✅       | ✅   | ❌   |
| Malagasy          | ✅       | ✅   | ✅   |
| Malay             | ✅       | ✅   | ✅   |
| Malayalam         | ✅       | ❌   | ❌   |
| Maltese           | ✅       | ✅   | ✅   |
| Maori             | ✅       | ✅   | ✅   |
| Marathi           | ✅       | ❌   | ❌   |
| Mari              | ✅       | ✅   | ❌   |
| Mongolian         | ✅       | ❌   | ❌   |
| Nepali            | ✅       | ❌   | ❌   |
| Norwegian         | ✅       | ✅   | ✅   |
| Papiamento        | ✅       | ✅   | ✅   |
| Polish            | ✅       | ✅   | ✅   |
| Portuguese Brazil | ✅       | ✅   | ✅   |
| Punjabi           | ✅       | ❌   | ❌   |
| Romanian          | ✅       | ✅   | ✅   |
| Russian           | ✅       | ✅   | ✅   |
| Scottish          | ✅       | ✅   | ✅   |
| Serbian           | ✅       | ✅   | ❌   |
| Sinhala           | ✅       | ❌   | ❌   |
| Slovakian         | ✅       | ✅   | ✅   |
| Swahili           | ❌       | ✅   | ✅   |
| Slovenian         | ✅       | ✅   | ✅   |
| Spanish           | ✅       | ✅   | ✅   |
| Sudanese          | ✅       | ✅   | ✅   |
| Swedish           | ✅       | ✅   | ✅   |
| Tagalog           | ✅       | ✅   | ✅   |
| Tajik             | ✅       | ✅   | ❌   |
| Tamil             | ✅       | ❌   | ❌   |
| Tatar             | ✅       | ✅   | ❌   |
| Telugu            | ✅       | ❌   | ❌   |
| Thai              | ✅       | ✅   | ✅   |
| Turkish           | ✅       | ✅   | ✅   |
| Udmurt            | ✅       | ❌   | ❌   |
| Ukrainian         | ✅       | ✅   | ❌   |
| Urdu              | ✅       | ❌   | ❌   |
| Uzbek             | ✅       | ✅   | ✅   |
| Vietnamese        | ✅       | ✅   | ✅   |
| Xhosa             | ✅       | ✅   | ✅   |

## Translation

Translate a piece of text. This block is powered by Yandex. Any language code from [this list ](https://yandex.com/dev/translate/doc/dg/concepts/api-overview.html)can be used.

![](<.gitbook/assets/image (139).png>)

## Recognize Speech

Recognize a piece of audio in a given language. Returns a text transcription of the speech.

![](<.gitbook/assets/image (155).png>)
