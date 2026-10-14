---
title: "SevenZipLZMACompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات طريقة ضغط LZMA داخل أرشيف 7z."
type: docs
weight: 115
url: /ar/java/com.aspose.zip/sevenziplzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMACompressionSettings extends SevenZipCompressionSettings
```

إعدادات طريقة ضغط LZMA داخل أرشيف 7z.

خوارزمية Lempel\u2013Ziv\u2013Markov chain (LZMA) هي خوارزمية تُستخدم لتنفيذ ضغط البيانات بدون فقدان. تستخدم هذه الخوارزمية مخطط ضغط القاموس مشابه إلى حد ما لخوارزمية LZ77 وتتميز بنسبة ضغط عالية وحجم قاموس ضغط متغير.

المزيد: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SevenZipLZMACompressionSettings()](#SevenZipLZMACompressionSettings--) | يُنشئ مثيلًا جديدًا من الفئة [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) مع المعلمات الافتراضية. |
| [SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#SevenZipLZMACompressionSettings-int-int-int-) | يُنشئ مثيلًا جديدًا من الفئة [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) مع حجم القاموس المحدد، وعدد البايتات السريعة، وعدد بتات سياق الحرف الحرفي. |
| [SevenZipLZMACompressionSettings(int dictionarySize)](#SevenZipLZMACompressionSettings-int-) | يُنشئ مثيلًا جديدًا من الفئة [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) مع حجم القاموس المحدد، وعدد البايتات السريعة يساوي 32، وعدد بتات سياق الحرف الحرفي يساوي 3. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | حجم القاموس (مخزن التاريخ) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحفظ في الذاكرة. |
| [getLiteralContextBits()](#getLiteralContextBits--) | يحصل على عدد بتات السياق الحرفي. |
| [getMethod()](#getMethod--) | يحصل على طريقة الضغط أو الفك. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | يحصل على عدد البايتات المستخدمة للبحث السريع عن التطابق في خوارزمية LZMA. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | حجم القاموس (مخزن التاريخ) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحفظ في الذاكرة. |
### SevenZipLZMACompressionSettings() {#SevenZipLZMACompressionSettings--}
```
public SevenZipLZMACompressionSettings()
```


يُنشئ مثيلًا جديدًا من الفئة [SevenZipLZMACompressionSettings](../../com.aspose.zip/sevenziplzmacompressionsettings) مع المعلمات الافتراضية.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save(\"result.7z\");
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

