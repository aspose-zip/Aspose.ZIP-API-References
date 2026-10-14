---
title: "SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "7z अभिलेख में LZMA संपीड़न विधि के लिए सेटिंग्स।"
type: docs
weight: 115
url: /hi/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

7z अभिलेख में LZMA संपीड़न विधि के लिए सेटिंग्स।

Lempel–Ziv–Markov श्रृंखला एल्गोरिद्म (LZMA) एक एल्गोरिद्म है जो नुकसान‑रहित डेटा संपीड़न करने के लिए उपयोग किया जाता है। यह एल्गोरिद्म एक शब्दकोश संपीड़न योजना का उपयोग करता है जो LZ77 एल्गोरिद्म के समान है और उच्च संपीड़न अनुपात तथा परिवर्तनीय संपीड़न‑शब्दकोश आकार प्रदान करता है।

और अधिक देखें: [Lempel–Ziv–Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | डिफ़ॉल्ट पैरामीटरों के साथ [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) क्लास का नया उदाहरण आरंभ करता है। |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | निर्दिष्ट शब्दकोश आकार, तेज़ बाइट्स की संख्या और लिटरल कॉन्टेक्स्ट बिट्स की संख्या के साथ [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) क्लास का नया उदाहरण आरंभ करता है। |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | निर्दिष्ट शब्दकोश आकार, तेज़ बाइट्स की संख्या 32 के बराबर, और लिटरल कॉन्टेक्स्ट बिट्स की संख्या 3 के बराबर के साथ [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) क्लास का नया उदाहरण आरंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | डिक्शनरी (इतिहास बफ़र) आकार यह दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। |
| [getLiteralContextBits()](#getLiteralContextBits--) | लिटरल कॉन्टेक्स्ट बिट्स की संख्या प्राप्त करता है। |
| [getMethod()](#getMethod--) | संपीड़न या डिकम्प्रेशन विधि प्राप्त करता है। |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | LZMA एल्गोरिद्म में तेज़ मैच खोज के लिए उपयोग किए जाने वाले बाइट्स की संख्या प्राप्त करता है। |
| [setDictionarySize(int value)](#setDictionarySize-int-) | डिक्शनरी (इतिहास बफ़र) आकार यह दर्शाता है कि हाल ही में प्रोसेस किए गए अनकम्प्रेस्ड डेटा के कितने बाइट्स मेमोरी में रखे जाते हैं। |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


डिफ़ॉल्ट पैरामीटरों के साथ [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) क्लास का नया उदाहरण आरंभ करता है।

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("result.7z");
}
 
```



### SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits) {#SevenZipLZMACompressionSettings-int-int-int-}
```
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```


Initializes a new instance of the [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) class with specified dictionary size, number of fast bytes and number of literal context bits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |
| numberOfFastBytes | int | The number of bytes used for fast match searching in the LZMA algorithm. Can be in the range from 5 to 273. |
| literalContextBits | int | Sets the number of literal context bits (high bits of previous literal). It can be in range from 0 to 8. |

### SevenZipLZMACompressionSettings(int dictionarySize) {#SevenZipLZMACompressionSettings-int-}
```
public SevenZipLZMACompressionSettings(int dictionarySize)
```


Initializes a new instance of the [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) class with specified dictionary size, number of fast bytes equal to 32, number of literal context bits equal to 3.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dictionarySize | int | Dictionary (history buffer) size in bytes. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size. |

### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Returns:**
int - dictionary (history buffer) size
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


Gets the number of literal context bits.

Literal Context Bits define how many of the most significant bits of the previous uncompressed byte are used to predict the bits of the next literal byte. Must be from 0 to 8.

**Returns:**
int - the number of literal context bits.
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Gets compression or decompression method.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


Gets the number of bytes used for fast match searching in the LZMA algorithm.

A higher value allows the compressor to search longer matches, which can improve the compression ratio slightly but slows down compression.

**Returns:**
int - the number of bytes used for fast match searching in the LZMA algorithm.
### setDictionarySize(int value) {#setDictionarySize-int-}
```
public final void setDictionarySize(int value)
```


Dictionary (history buffer) size indicates how many bytes of the recently processed uncompressed data is kept in memory. If not set, will be chosen accordingly to entry size. Must be between 4096 and 1073741824, or equal to zero for automatic detection based on entry size.

The bigger the dictionary, usually the better the compression ratio is - but dictionaries larger than the uncompressed data are a waste of RAM.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | dictionary (history buffer) size |

