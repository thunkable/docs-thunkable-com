#### T**hunkable Cross-Platform **✕

# Speech Recognizer ![](/assets/iOSviewIconSpeechRecognizer.png)

---

The Speech Recognizer uses artificial intelligence to recognize and translate spoken language into text in 14 different languages.

The Speech Recognizer component can translate a full phrase or in real-time as a person is speaking. The Speech Recognizer stops listening after it stops detecting any sound. 

* [Translate a full phrase](#recognize-a-full-phrase)
* [Translate in real-time](/Recognize in real-time)

---

### Translate a full phrase

![](/assets/speech-recognizer-✕-fig-1.png)

| Event | Description |
| :--- | :--- |
| Listen \(`speech`\) | Returns a text `value` after a full phrase has been spoken. The Speech Recognizer stops listening after it stops detecting any sound. |

---

### Translate in real-time

![](/assets/speech-recognizer-✕-fig-2.png)

| Event | Description |
| :--- | :--- |
| Listen with Partial Result  \(`speech`\) | Returns a text `partialResult` in real-time as a phrase is being spoken. The Speech Recognizer stops listening after it stops detecting any sound. |



