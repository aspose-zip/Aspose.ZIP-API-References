---
title: "LzmaArchiveSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات أرشيف lzma."
type: docs
weight: 87
url: /ar/java/com.aspose.zip/lzmaarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class LzmaArchiveSettings
```

إعدادات أرشيف lzma.

خوارزمية Lempel\u2013Ziv\u2013Markov chain (LZMA) هي خوارزمية تُستخدم لتنفيذ ضغط البيانات بدون فقدان. تستخدم هذه الخوارزمية مخطط ضغط القاموس مشابه إلى حد ما لخوارزمية LZ77 وتتميز بنسبة ضغط عالية وحجم قاموس ضغط متغير.

المزيد: [Lempel\u2013Ziv\u2013Markov chain algorithm][Lempel_u2013Ziv_u2013Markov chain algorithm]


[Lempel_u2013Ziv_u2013Markov chain algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzmaArchiveSettings()](#LzmaArchiveSettings--) | ينشئ مثيلاً جديداً من الفئة [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) بحجم القاموس الافتراضي، والذي يساوي 16 ميغابايت، وعدد البايتات السريعة يساوي 32، وبتات السياق الحرفي تساوي 3. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionProgressed()](#getCompressionProgressed--) | يحصل على حدث يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [getDictionarySize()](#getDictionarySize--) | حجم القاموس (مخزن السجل) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحتفظ بها في الذاكرة. |
| [getLiteralContextBits()](#getLiteralContextBits--) | يحصل على عدد بتات السياق الحرفي. |
| [getNumberOfFastBytes()](#getNumberOfFastBytes--) | يحصل على عدد البايتات المستخدمة للبحث السريع عن التطابق في خوارزمية LZMA. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام. |
| [setDictionarySize(int value)](#setDictionarySize-int-) | حجم القاموس (مخزن السجل) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحتفظ بها في الذاكرة. |
| [setLiteralContextBits(int value)](#setLiteralContextBits-int-) | يضبط عدد بتات السياق الحرفي. |
| [setNumberOfFastBytes(int value)](#setNumberOfFastBytes-int-) | يضبط عدد البايتات المستخدمة للبحث السريع عن التطابق في خوارزمية LZMA. |
### LzmaArchiveSettings() {#LzmaArchiveSettings--}
```
public LzmaArchiveSettings()
```


ينشئ مثيلاً جديداً من الفئة [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) بحجم القاموس الافتراضي، والذي يساوي 16 ميغابايت، وعدد البايتات السريعة يساوي 32، وبتات السياق الحرفي تساوي 3.

```

``````

LzmaArchiveSettings settings = new LzmaArchiveSettings();
settings.setDictionarySize(1048576);
try (LzmaArchive archive = new LzmaArchive(settings)) {
archive.setSource(\"data.bin\");
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


يشير حجم Dictionary (history buffer) إلى عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحفظ في الذاكرة. إذا لم يتم تعيينه، سيتم اختياره وفقًا لحجم الإدخال.

كلما كان القاموس أكبر، عادةً ما تكون نسبة الضغط أفضل - لكن القواميس التي تتجاوز حجم البيانات غير المضغوطة تُعد إهدارًا للذاكرة العشوائية. يجب أن يكون حجم القاموس في أرشيف LZMA إما قوة اثنين (2^n) أو ثلاثة أضعاف قوة اثنين (3\*2^n).

**Returns:**
int - حجم Dictionary (history buffer).
### getLiteralContextBits() {#getLiteralContextBits--}
```
public final int getLiteralContextBits()
```


يحصل على عدد بتات السياق الحرفي.

تحدد Literal Context Bits عدد البتات الأكثر أهمية في البايت غير المضغوط السابق المستخدمة لتوقع بتات البايت الحرفي التالي. يجب أن تكون بين 0 و 8.

**Returns:**
int - عدد بتات السياق الحرفي.
### getNumberOfFastBytes() {#getNumberOfFastBytes--}
```
public final int getNumberOfFastBytes()
```


يحصل على عدد البايتات المستخدمة للبحث السريع عن التطابق في خوارزمية LZMA.

قيمة أعلى تسمح للضاغط بالبحث عن تطابقات أطول، مما يمكن أن يحسن نسبة الضغط قليلًا لكنه يبطئ عملية الضغط.

**Returns:**
int - عدد البايتات المستخدمة للبحث السريع عن التطابق في خوارزمية LZMA.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setCompressionProgressed(Event<ProgressEventArgs> value)
```


يضبط حدثًا يُرفع عندما يتم ضغط جزء من الدفق الخام.

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

