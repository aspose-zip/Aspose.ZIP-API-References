---
title: "LzmaCompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات طريقة ضغط LZMA."
type: docs
weight: 88
url: /ar/java/com.aspose.zip/lzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class LzmaCompressionSettings extends CompressionSettings
```

إعدادات طريقة ضغط LZMA.

خوارزمية Lempel\u2013Ziv\u2013Markov chain (LZMA) هي خوارزمية تُستخدم لتنفيذ ضغط البيانات بدون فقدان. تستخدم هذه الخوارزمية مخطط ضغط القاموس مشابه إلى حد ما لخوارزمية LZ77 وتتميز بنسبة ضغط عالية وحجم قاموس ضغط متغير.

المزيد: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzmaCompressionSettings()](#LzmaCompressionSettings--) | ينشئ نسخة جديدة من الفئة [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) باستخدام المعلمات الافتراضية. |
| [LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)](#LzmaCompressionSettings-int-int-int-) | ينشئ نسخة جديدة من الفئة [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) بحجم القاموس المحدد، وعدد البايتات السريعة، وعدد بتات سياق الحرف الحرفي. |
| [LzmaCompressionSettings(int dictionarySize)](#LzmaCompressionSettings-int-) | ينشئ نسخة جديدة من الفئة [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) بحجم القاموس المحدد، وعدد البايتات السريعة الافتراضي يساوي 32، وعدد بتات سياق الحرف الحرفي يساوي 3. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getDictionarySize()](#getDictionarySize--) | حجم القاموس (مخزن السجل) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحتفظ بها في الذاكرة. |
| [getLiteralContextBits()](#getLiteralContextBits--) | يحصل على عدد بتات السياق الحرفي. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | يحصل على عدد البايتات المستخدمة للبحث السريع عن التطابق في خوارزمية LZMA. |
### LzmaCompressionSettings() {#LzmaCompressionSettings--}
```
public LzmaCompressionSettings()
```


ينشئ نسخة جديدة من الفئة [LzmaCompressionSettings](../../com.aspose.zip/lzmacompressionsettings) باستخدام المعلمات الافتراضية.

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings()))) {
archive.createEntry(\"data.bin\", \"data.bin\");
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
