---
title: "IsoLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "الخيارات التي يتم من خلالها تحميل  من ملف مضغوط."
type: docs
weight: 73
url: /ar/java/com.aspose.zip/isoloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class IsoLoadOptions
```

الخيارات التي يتم من خلالها تحميل [IsoArchive](../../com.aspose.zip/isoarchive) من ملف مضغوط. يحتوي على الحدث المثار عند الاستخراج.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [IsoLoadOptions()](#IsoLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات. |
### IsoLoadOptions() {#IsoLoadOptions--}
```
public IsoLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات.

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive("archive.iso", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel ISO archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         IsoLoadOptions options = new IsoLoadOptions();
         options.setCancellationFlag(cf);
         try (IsoArchive a = new IsoArchive("big.iso", options)) {
             try {
                 a.getEntries().get(0).extract("data.bin");
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

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات.

```

``````

long length = 10_000_000;
IsoLoadOptions loadOptions = new IsoLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / length);
});
IsoArchive archive = new IsoArchive("archive.iso", loadOptions);
 
```

Event sender is the [IsoEntry](../../com.aspose.zip/isoentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

