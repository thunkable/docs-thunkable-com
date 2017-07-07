#### **Thunkable for Android **❤

# Yandex Translate

---

Yandex Translate is a powerful service that translate spoken or typed text into 90+ languages almost instantly. This component needs Internet access, as it will request translations to the Yandex Translate service. See http://api.yandex.com/translate/ for more information

The Yandex Translate component is used in the sample app [ThunkableChat: Chat with Instant Translation](https://www.gitbook.com/book/albertching/thunkable-docs/edit#)

---

#### Translate spoken text to Russian

![](/assets/yandex-translate-blocks.png)

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Request Translation \(language to Translate to, text to translate\) | Requests a translation to the Yandex Translate service given some text to translate and a language to translate the text to. The language must be specified in 2 digit codes e.g. 'en' for English and the list of supported languages is listed below. Yandex Translate will attempt to detect the source language. You can also specify the language to translate from i.e. 'es-ru' will specify Spanish to Russian |
| Got Translation \(responseCode, translation\) | Event triggered when the Yandex Translate service returns the translated text. The even also provides a response code for error handling. If the responseCode is not 200, then something went wrong and no translation will be available |
| Yandex Key | Thunkable is providing its own key by DEFAULT. You can sign up for your own key on Yandex |

---

#### Available translation languages

According to [Yandex](https://tech.yandex.com/translate/doc/dg/concepts/api-overview-docpage/#languages), there are more than 90 available languages including the ones below

|  | Language code |
| :--- | :--- |
| Bangla | bn |
| Czech | cs |
| Danish | da |
| Dutch | nl |
| English | en |
| Finnish | fi |
| French | fr |
| German | de |
| Hindi | hi |
| Hungarian | hu |
| Indonesian | in |
| Italian | it |
| Japanese | ja |
| Khmer | km |
| Korean | ko |
| Mandarin Chinese | zh |
| Nepali | ne |
| Norwegian | no |
| Polish | pl |
| Portuguese | pt |
| Russian | ru |
| Sinhala | si |
| Spanish | es |
| Swedish | sv |
| Thai | th |
| Turkish | tr |
| Ukranian | uk |
| Vietnamese | vi |

#### 



