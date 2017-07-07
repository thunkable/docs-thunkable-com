#### **Thunkable for Android **❤

# Text to Speech

---

The Text to Speech component speaks a given text aloud. You can set the pitch and the rate of speech because the speech is synthesized from human speech.

You can also change the pronunciation of words \(not the actual language spoken\) by supplying a language or country code. For example, setting the language to French and speaking English text will sound like someone speaking English \(en\) with a French accent. Setting the country code to British English \(GBR\) will sound different from US English \(USA\) and not every country code will affect every language

The languages and countries available depend on the particular device, and can be listed with the Available Languages and Available Countries properties.

The Text to Speech component is used in the sample app [ThunkableChat: Chat with Instant Translation](https://www.gitbook.com/book/albertching/thunkable-docs/edit#)

---

#### Speak text with a Mandarin Chinese pronunciation

![](/assets/text-to-speech-blocks.png)

---

#### Sound

| Property | Description |
| :--- | :--- |
| Language | Sets the language in which the text is pronounced but does not change the content of the language that is spoken. For example, setting the language to French and speaking English text will sound like someone speaking English with a French accent. The list of available languages are below |
| Country | Sets the country in which the text may be pronounced but does not change the content of the language that is spoken. For example, British English will sound different from US English. Not every country will affect every language. The list of available countries are below |
| Pitch | Between 0 and 2, where lower values lower the tone of the synthesized voice and greater values raise it |
| Available Languages | More languages are available than shown in Designer drop down. See below for latest |
| Available Countries | Designer drop down shows more options than currently supported. See below for latest |

---

#### Available pronunciation languages

According to [this article](https://en.wikipedia.org/wiki/Google_Text-to-Speech), below are the available language and countries for Text to Speech

|  | Language code | Country code |
| :--- | :--- | :--- |
| Bangla \(Bangladesh, India\) | bn | BGD, IND |
| Czech | cs |  |
| Danish | da |  |
| Dutch | nl |  |
| English \(Australia, India, United Kingdom, USA\) | en | AUS, IND, GBR, USA |
| Finnish | fi |  |
| French | fr |  |
| German | de |  |
| Hindi | hi |  |
| Hungarian | hu |  |
| Indonesian | in |  |
| Italian | it |  |
| Japanese | ja |  |
| Khmer | km |  |
| Korean | ko |  |
| Mandarin Chinese \(China, Taiwan\) | zh | CHN, TWN |
| Nepali | ne |  |
| Norwegian | no |  |
| Polish | pl |  |
| Portuguese \(Brazil\) | pt |  |
| Russian | ru |  |
| Sinhala | si |  |
| Spanish \(Spain, USA\) | es | ESP, USA |
| Swedish | sv |  |
| Thai | th |  |
| Turkish | tr |  |
| Ukranian | uk |  |
| Vietnamese | vi |  |

---

#### Functionality

| Event | Description |
| :--- | :--- |
| Speak \(message\) | Converts a text 'message' into speech |
| Before Speaking | Before the text is spoken |
| After Speaking \(result\) | After the text is spoken, the 'result' refers to the spoken text |



