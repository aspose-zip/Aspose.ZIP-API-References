---
title: "LzipLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات التحميل ."
type: docs
weight: 85
url: /ar/java/com.aspose.zip/lziploadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LzipLoadOptions
```

خيارات تحميل [LzipArchive](../../com.aspose.zip/lziparchive).

في إطار عمل .NET Framework 4.0 وما فوق، يمكن استخدامها لإلغاء الاستخراج.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LzipLoadOptions()](#LzipLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
### LzipLoadOptions() {#LzipLoadOptions--}
```
public LzipLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج.

إلغاء استخراج أرشيف lzip بعد وقت معين.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LzipLoadOptions options = new LzipLoadOptions();
options.setCancellationFlag(cf);
try (LzipArchive a = new LzipArchive("big.lz", options)) {
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

