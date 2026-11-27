---
title: "SevenZipLZMA2CompressionSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z."
type: docs
weight: 114
url: /ar/java/com.aspose.zip/sevenziplzma2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipLZMA2CompressionSettings extends SevenZipCompressionSettings
```

إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z.

يدعم LZMA2 عدة عمليات للبيانات المضغوطة بتنسيق LZMA والبيانات غير المضغوطة.

المزيد: [Lempel\\u2013Ziv\\u2013Markov\_chain\_algorithm][Lempel_u2013Ziv_u2013Markov_chain_algorithm]


[Lempel_u2013Ziv_u2013Markov_chain_algorithm]: https://en.wikipedia.org/wiki/Lempel\u2013Ziv\u2013Markov_chain_algorithm
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [SevenZipLZMA2CompressionSettings()](#SevenZipLZMA2CompressionSettings--) | ينشئ إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize)](#SevenZipLZMA2CompressionSettings-int-) | ينشئ إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z. |
| [SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)](#SevenZipLZMA2CompressionSettings-int-int-) | ينشئ إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | يحصل على عدد خيوط الضغط. |
| [getDictionarySize()](#getDictionarySize--) | حجم القاموس (مخزن السجل) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحتفظ بها في الذاكرة. |
| [getFastBytes()](#getFastBytes--) | يحصل على رقم التحكم للبايتات السريعة المستخدمة بواسطة ضاغط LZMA2. |
| [getMethod()](#getMethod--) | يحصل على طريقة الضغط أو الفك. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | يضبط عدد خيوط الضغط. |
### SevenZipLZMA2CompressionSettings() {#SevenZipLZMA2CompressionSettings--}
```
public SevenZipLZMA2CompressionSettings()
```


ينشئ إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z.

### SevenZipLZMA2CompressionSettings(int dictionarySize) {#SevenZipLZMA2CompressionSettings-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize)
```


ينشئ إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | dictionarySize | int | حجم مخزن التاريخ، يجب أن يكون بين 4096 و 1073741824. |

كلما كان القاموس أكبر، عادةً ما تكون نسبة الضغط أفضل - لكن القواميس التي تتجاوز حجم البيانات غير المضغوطة تُهدر الذاكرة العشوائية. |

### SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes) {#SevenZipLZMA2CompressionSettings-int-int-}
```
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes)
```


ينشئ إعدادات طريقة ضغط LZMA2 داخل أرشيف 7z.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | dictionarySize | int | حجم مخزن التاريخ، يجب أن يكون بين 4096 و 1073741824. |

كلما كان القاموس أكبر، عادةً ما تكون نسبة الضغط أفضل - لكن القواميس التي تتجاوز حجم البيانات غير المضغوطة تُهدر الذاكرة العشوائية. |
| fastBytes | int | يتحكم في عدد البايتات السريعة المستخدمة بواسطة ضاغطات LZMA2. يمكن لعدد أكبر من البايتات السريعة أن يوفر نسبة ضغط أفضل على حساب سرعة الضغط. |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


يحصل على عدد خيوط الضغط. إذا كانت القيمة أكبر من 1، سيتم استخدام ضغط متعدد الخيوط.

**Returns:**
int - عدد خيوط الضغط
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


حجم القاموس (مخزن السجل) يوضح عدد البايتات من البيانات غير المضغوطة التي تمت معالجتها مؤخرًا والتي تُحتفظ بها في الذاكرة.

**Returns:**
int - حجم القاموس (مخزن التاريخ)
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


يحصل على رقم التحكم للبايتات السريعة المستخدمة بواسطة ضاغط LZMA2.

**Returns:**
int - عدد التحكم للبايتات السريعة المستخدمة بواسطة ضاغط LZMA2
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


يحصل على طريقة الضغط أو الفك.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method.
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


يضبط عدد خيوط الضغط. إذا كانت القيمة أكبر من 1، سيتم استخدام الضغط متعدد الخيوط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | عدد خيوط الضغط. |

لا تقم بتعيين هذا الرقم أكثر من نوى المعالج. |

