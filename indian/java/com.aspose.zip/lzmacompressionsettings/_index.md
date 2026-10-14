---
title: "LzmaCompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "LZMA संपीड़न विधि के लिए सेटिंग्स।"
type: docs
weight: 88
url: /hi/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

LZMA संपीड़न विधि के लिए सेटिंग्स।

Lempel–Ziv–Markov श्रृंखला एल्गोरिद्म (LZMA) एक एल्गोरिद्म है जो नुकसान‑रहित डेटा संपीड़न करने के लिए उपयोग किया जाता है। यह एल्गोरिद्म एक शब्दकोश संपीड़न योजना का उपयोग करता है जो LZ77 एल्गोरिद्म के समान है और उच्च संपीड़न अनुपात तथा परिवर्तनीय संपीड़न‑शब्दकोश आकार प्रदान करता है।

और अधिक देखें: [Lempel–Ziv–Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | डिफ़ॉल्ट पैरामीटर के साथ [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | निर्दिष्ट डिक्शनरी आकार, फास्ट बाइट्स की संख्या और लिटरल कॉन्टेक्स्ट बिट्स की संख्या के साथ [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | निर्दिष्ट डिक्शनरी आकार, डिफ़ॉल्ट फास्ट बाइट्स की संख्या 32 और लिटरल कॉन्टेक्स्ट बिट्स की संख्या 3 के साथ [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | डिक्शनरी (इतिहास बफ़र) आकार दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। |
| [getLiteralContextBits()](#getLiteralContextBits--) | लिटरल कॉन्टेक्स्ट बिट्स की संख्या प्राप्त करता है। |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA एल्गोरिद्म में तेज़ मैच खोज के लिए उपयोग किए जाने वाले बाइट्स की संख्या प्राप्त करता है। |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


डिफ़ॉल्ट पैरामीटर के साथ [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



### LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#LzmaCompressionSettings-int-int-int-}
```
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### LzmaCompressionSettings(int dictionarySize) {#LzmaCompressionSettings-int-}
```
public LzmaCompressionSettings(int dictionarySize)
```


Initializes a new instance of the [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) class with specified dictionary size, default number of fast bytes equal to 32 and number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data are kept in memory.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - how many bytes of the recently processed uncompressed data are kept in memory.
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
