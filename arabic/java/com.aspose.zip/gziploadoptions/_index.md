---
title: "GzipLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات التحميل ."
type: docs
weight: 70
url: /ar/java/com.aspose.zip/gziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class GzipLoadOptions
```

خيارات التحميل [GzipArchive](../../com.aspose.zip/gziparchive).

في إطار عمل .NET Framework 4.0 وما فوق، يمكن استخدامها لإلغاء الاستخراج.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [GzipLoadOptions()](#GzipLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getParseHeader()](#getParseHeader--) | يحصل على القيمة التي تشير إلى ما إذا كان يجب تحليل رأس الدفق لاستخلاص الخصائص، بما في ذلك الاسم. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
| [setParseHeader(boolean value)](#setParseHeader-boolean-) | يضبط القيمة التي تشير إلى ما إذا كان يجب تحليل رأس الدفق لاستخلاص الخصائص، بما في ذلك الاسم. |
### GzipLoadOptions() {#GzipLoadOptions--}
```
public GzipLoadOptions()
```


### getParseHeader() {#getParseHeader--}
```
public final boolean getParseHeader()
```


يحصل على القيمة التي تشير إلى ما إذا كان يجب تحليل رأس الدفق لاستخلاص الخصائص، بما في ذلك الاسم. يكون ذلك منطقيًا فقط للدفق القابل للتمرير.

**Returns:**
منطقي - القيمة التي تشير إلى ما إذا كان يجب تحليل رأس الدفق لاستخلاص الخصائص، بما في ذلك الاسم.
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج.

إلغاء استخراج أرشيف gzip بعد فترة زمنية معينة.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
GzipLoadOptions options = new GzipLoadOptions();
options.setCancellationFlag(cf);
try (GzipArchive a = new GzipArchive("big.gz", options)) {
try {
a.extract("data.bin");
} catch (OperationCanceledException e) {
System.out.println("تم إلغاء الاستخراج بعد 60 ثانية");
}
}
}
 
```

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setParseHeader(boolean value) {#setParseHeader-boolean-}
```
public final void setParseHeader(boolean value)
```


Sets the value indicating whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | the value indicating whether to parse stream header to figure out properties, including name. |

