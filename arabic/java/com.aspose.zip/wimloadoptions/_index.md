---
title: "WimLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الخيارات التي يتم من خلالها تحميل الأرشيف من ملف مضغوط."
type: docs
weight: 135
url: /ar/java/com.aspose.zip/wimloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class WimLoadOptions
```

الخيارات التي يتم من خلالها تحميل الأرشيف من ملف مضغوط.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [WimLoadOptions()](#WimLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
### WimLoadOptions() {#WimLoadOptions--}
```
public WimLoadOptions()
```


### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج.

إلغاء استخراج أرشيف WIM بعد وقت معين.

```

``````

try (CancellationFlag cf = new CancellationFlag()) {
cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
WimLoadOptions options = new WimLoadOptions();
options.setCancellationFlag(cf);
try (WimArchive a = new WimArchive("big.wim", options)) {
try {
StreamSupport.stream(a.getImages().get(0).getAllEntries().spliterator(), false)
.filter(entry -> entry instanceof WimFileEntry)
.map(entry -> (WimFileEntry) entry)
.findFirst().ifPresent(entry -> entry.extract("data.bin"));
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

