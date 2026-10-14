---
title: "LzmaArchiveSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "lzma आर्काइव के लिए सेटिंग्स।"
type: docs
weight: 87
url: /hi/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

lzma आर्काइव के लिए सेटिंग्स।

Lempel–Ziv–Markov श्रृंखला एल्गोरिद्म (LZMA) एक एल्गोरिद्म है जो नुकसान‑रहित डेटा संपीड़न करने के लिए उपयोग किया जाता है। यह एल्गोरिद्म एक शब्दकोश संपीड़न योजना का उपयोग करता है जो LZ77 एल्गोरिद्म के समान है और उच्च संपीड़न अनुपात तथा परिवर्तनीय संपीड़न‑शब्दकोश आकार प्रदान करता है।

और अधिक देखें: [Lempel–Ziv–Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | डिफ़ॉल्ट शब्दकोश आकार, 16 मेगाबाइट, तेज़ बाइट्स की संख्या 32 और लिटरल कॉन्टेक्स्ट बिट्स 3 के साथ [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) क्लास का नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को प्राप्त करता है। |
| [getDictionarySize()](#getDictionarySize--) | डिक्शनरी (इतिहास बफ़र) आकार दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। |
| [getLiteralContextBits()](#getLiteralContextBits--) | लिटरल कॉन्टेक्स्ट बिट्स की संख्या प्राप्त करता है। |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA एल्गोरिद्म में तेज़ मैच खोज के लिए उपयोग किए जाने वाले बाइट्स की संख्या प्राप्त करता है। |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को सेट करता है। |
| [setDictionarySize(int value)](#setDictionarySize-int-) | डिक्शनरी (इतिहास बफ़र) आकार दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | लिटरल कॉन्टेक्स्ट बिट्स की संख्या सेट करता है। |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | LZMA एल्गोरिद्म में तेज़ मैच खोज के लिए उपयोग किए जाने वाले बाइट्स की संख्या सेट करता है। |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


डिफ़ॉल्ट शब्दकोश आकार, 16 मेगाबाइट, तेज़ बाइट्स की संख्या 32 और लिटरल कॉन्टेक्स्ट बिट्स 3 के साथ [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) क्लास का नया उदाहरण प्रारंभ करता है।

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource("data.bin");
archive.save(lzmaFile);
}
 
```



### getCompressionProgressed() {#getCompressionProgressed--}
```
public Event<ProgressEventArgs> getCompressionProgressed()
```


Gets an event that is raised when a portion of raw stream compressed.

```

``````

    lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```



**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


डिक्शनरी (इतिहास बफ़र) आकार दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। यदि सेट नहीं किया गया, तो यह एंट्री आकार के अनुसार चुना जाएगा।

जितनी बड़ी डिक्शनरी होगी, आमतौर पर संपीड़न अनुपात उतना ही बेहतर होता है - लेकिन अनकम्प्रेस्ड डेटा से बड़ी डिक्शनरी RAM की बर्बादी है। LZMA आर्काइव का डिक्शनरी आकार या तो दो की शक्ति (2^n) होना चाहिए या दो की शक्ति का तीन गुना (3*2^n)।

**Returns:**
int - डिक्शनरी (इतिहास बफ़र) आकार।
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


लिटरल कॉन्टेक्स्ट बिट्स की संख्या प्राप्त करता है।

लिटरल कॉन्टेक्स्ट बिट्स निर्धारित करते हैं कि पिछले अनकम्प्रेस्ड बाइट के सबसे महत्वपूर्ण बिट्स में से कितने बिट्स अगले लिटरल बाइट के बिट्स की भविष्यवाणी करने के लिए उपयोग होते हैं। मान 0 से 8 के बीच होना चाहिए।

**Returns:**
int - लिटरल कॉन्टेक्स्ट बिट्स की संख्या।
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


LZMA एल्गोरिद्म में तेज़ मैच खोज के लिए उपयोग किए जाने वाले बाइट्स की संख्या प्राप्त करता है।

उच्च मान कम्प्रेसर को लंबी मैच खोजने की अनुमति देता है, जिससे संपीड़न अनुपात थोड़ा सुधार सकता है लेकिन संपीड़न गति धीमी हो जाती है।

**Returns:**
int - LZMA एल्गोरिदम में तेज़ मिलान खोज के लिए उपयोग किए जाने वाले बाइट्स की संख्या।
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


जब कच्चे स्ट्रीम का एक भाग संकुचित होता है तो उठाए जाने वाले इवेंट को सेट करता है।

```

``````

lzmaArchiveSettings.setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory. If not set, will be chosen accordingly to entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM. The disctionary size of LZMA archive must be either a power of two (2^n) or three times a power of two (3\*2^n).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Dictionary (history buffer) size. |

### setLiteralContextBits(int value) {#setLiteralContextBits-int-}
```
public final void setLiteralContextBits(int value)
```


Sets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of literal context bits. |

### setNumberOfFastBytes(int value) {#setNumberOfFastBytes-int-}
```
public final void setNumberOfFastBytes(int value)
```


Sets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the number of bytes used for fast match searching in the LZMA algorithm. |

