---
title: "FastLZOutputStream"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "مغلف تدفق يضغط البيانات باستخدام FastLZ."
type: docs
weight: 68
url: /ar/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

مغلف تدفق يضغط البيانات باستخدام FastLZ. ينفذ نمط الزخرفة.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | يُنشئ مثيلاً جديدًا من الفئة FastLZStream المُعد للضغط. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [close()](#close--) | يغلق الدفق الحالي ويحرّر أي موارد (مثل المقابس ومقابض الملفات) المرتبطة بالدفق الحالي. |
| [flush()](#flush--) | يمسح جميع المخازن المؤقتة لهذا الدفق ويتسبب في كتابة أي بيانات مخزنة مؤقتًا إلى الجهاز الأساسي. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | يكتب تسلسلًا من البايتات إلى الدفق الضاغط ويتقدم بالموقع الحالي داخل هذا الدفق بعدد البايتات المكتوبة. |
| [write(int b)](#write-int-) | يكتب البايت المحدد إلى دفق الإخراج هذا. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


يُنشئ مثيلاً جديدًا من الفئة FastLZStream المُعد للضغط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | java.io.OutputStream | الدفق لحفظ البيانات المضغوطة |
| compressionLevel | int | استخدم 1 لضغط أسرع، واستخدم 2 لنسبة ضغط أفضل. |

### close() {#close--}
```
public void close()
```


يغلق الدفق الحالي ويحرّر أي موارد (مثل المقابس ومقابض الملفات) المرتبطة بالدفق الحالي.

### flush() {#flush--}
```
public void flush()
```


يمسح جميع المخازن المؤقتة لهذا الدفق ويتسبب في كتابة أي بيانات مخزنة مؤقتًا إلى الجهاز الأساسي.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


يكتب تسلسلًا من البايتات إلى الدفق الضاغط ويتقدم بالموقع الحالي داخل هذا الدفق بعدد البايتات المكتوبة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| buffer | byte[] | مصفوفة من البايتات. تنسخ هذه الطريقة عدد count من البايتات من المخزن المؤقت إلى الدفق الحالي. |
| offset | int | الإزاحة الصفرية للبايت في المخزن المؤقت التي يبدأ عندها نسخ البايتات إلى الدفق الحالي. |
| count | int | عدد البايتات التي ستُكتب إلى الدفق الحالي. |

### write(int b) {#write-int-}
```
public void write(int b)
```


يكتب البايت المحدد إلى دفق الإخراج هذا. العقد العام لـ `write` هو أن يتم كتابة بايت واحد إلى دفق الإخراج. البايت الذي سيُكتب هو الثمانية بتات الأقل ترتيبًا من الوسيط `b`. يتم تجاهل الـ 24 بتًا الأعلى ترتيبًا من `b`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| b | int | ال `byte` |

