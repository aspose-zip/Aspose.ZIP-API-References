---
title: "ZstandardLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الخيارات التي يتم من خلالها تحميل  من ملف مضغوط."
type: docs
weight: 158
url: /ar/java/com.aspose.zip/zstandardloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardLoadOptions
```

الخيارات التي يتم من خلالها تحميل [ZstandardArchive](../../com.aspose.zip/zstandardarchive) من ملف مضغوط. يحتوي على الحدث المثار عند الاستخراج.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [ZstandardLoadOptions()](#ZstandardLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات. |
### ZstandardLoadOptions() {#ZstandardLoadOptions--}
```
public ZstandardLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات.

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Zstandard archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZstandardLoadOptions options = new ZstandardLoadOptions();
         options.setCancellationFlag(cf);
         try (ZstandardArchive a = new ZstandardArchive("big.zstd", options)) {
             try {
                 a.extract("data.bin");
             } catch (OperationCanceledException e) {
                 System.out.println("Extraction was cancelled after 60 seconds");
             }
         }
     }
 
```

الإلغاء غالبًا ما يؤدي إلى عدم استخراج بعض البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | علامة إلغاء تُستخدم لإلغاء عملية الاستخراج. |

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات.

```

``````

long length = 10_000_000;
ZStandardLoadOptions loadOptions = new ZStandardLoadOptions();
loadOptions.setExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
ZstandardArchive archive = new ZstandardArchive("archive.zst", loadOptions);
 
```

Event sender is the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

