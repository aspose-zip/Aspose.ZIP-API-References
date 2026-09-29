---
title: "LhaLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الخيارات التي يتم من خلالها تحميل الأرشيف من ملف مضغوط."
type: docs
weight: 78
url: /ar/java/com.aspose.zip/lhaloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LhaLoadOptions
```

الخيارات التي يتم من خلالها تحميل الأرشيف من ملف مضغوط.

في إطار عمل .NET Framework 4.0 وما فوق، يمكن استخدامها لإلغاء الاستخراج.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [LhaLoadOptions()](#LhaLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
### LhaLoadOptions() {#LhaLoadOptions--}
```
public LhaLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج.

إلغاء استخراج أرشيف LHA بعد فترة زمنية معينة.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
LhaLoadOptions options = new LhaLoadOptions();
options.setCancellationFlag(cf);
try (LhaArchive a = new LhaArchive("big.lha", options)) {
try {
a.getEntries().get(0).extract("data.bin");
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

