---
title: "SevenZipLZMA2CompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z अभिलेख में LZMA2 संपीड़न विधि के लिए सेटिंग्स।"
type: docs
weight: 114
url: /hi/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

7z अभिलेख में LZMA2 संपीड़न विधि के लिए सेटिंग्स।

LZMA2 संकुचित LZMA डेटा और असंकुचित डेटा के कई रन को समर्थन देता है।

और देखें: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | 7z आर्काइव के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | 7z आर्काइव के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | 7z आर्काइव के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | कम्प्रेशन थ्रेड की संख्या प्राप्त करता है। |
| [getDictionarySize()](#getDictionarySize--) | डिक्शनरी (इतिहास बफ़र) आकार दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। |
| [getFastBytes()](#getFastBytes--) | LZMA2 संपीड़क द्वारा उपयोग किए गए फास्ट बाइट्स की नियंत्रण संख्या प्राप्त करता है। |
| [getMethod()](#getMethod--) | संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है। |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | कम्प्रेशन थ्रेड की संख्या सेट करता है। |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


7z आर्काइव के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है।

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


7z आर्काइव के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dictionarySize | int | इतिहास बफ़र का आकार, 4096 और 1073741824 के बीच होना चाहिए। |

डिक्शनरी जितनी बड़ी होगी, आमतौर पर संपीड़न अनुपात उतना ही बेहतर होगा - लेकिन असंकुचित डेटा से बड़ी डिक्शनरी RAM की बर्बादी है। |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


7z आर्काइव के भीतर LZMA2 संपीड़न विधि के लिए सेटिंग्स को इंस्टैंसिएट करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dictionarySize | int | इतिहास बफ़र का आकार, 4096 और 1073741824 के बीच होना चाहिए। |

डिक्शनरी जितनी बड़ी होगी, आमतौर पर संपीड़न अनुपात उतना ही बेहतर होगा - लेकिन असंकुचित डेटा से बड़ी डिक्शनरी RAM की बर्बादी है। |
| fastBytes | int | LZMA2 संपीड़कों द्वारा उपयोग किए गए फास्ट बाइट्स की संख्या को नियंत्रित करता है। फास्ट बाइट्स की बड़ी संख्या संपीड़न गति के खर्च पर बेहतर संपीड़न अनुपात प्रदान कर सकती है। |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


संपीड़न थ्रेड की संख्या प्राप्त करता है। यदि मान 1 से बड़ा है, तो मल्टीथ्रेडिंग संपीड़न उपयोग किया जाएगा।

**Returns:**
int - संपीड़न थ्रेड की संख्या
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


डिक्शनरी (इतिहास बफ़र) आकार दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं।

**Returns:**
int - डिक्शनरी (इतिहास बफ़र) आकार
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


LZMA2 संपीड़क द्वारा उपयोग किए गए फास्ट बाइट्स की नियंत्रण संख्या प्राप्त करता है।

**Returns:**
int - LZMA2 संपीड़क द्वारा उपयोग किए गए फास्ट बाइट्स की नियंत्रण संख्या
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है।

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


कम्प्रेशन थ्रेड की संख्या सेट करता है। यदि मान 1 से बड़ा है, तो मल्टीथ्रेडिंग कम्प्रेशन उपयोग किया जाएगा।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | कम्प्रेशन थ्रेड की संख्या। |

इस संख्या को CPU कोर से अधिक सेट न करें। |

