---
title: "XarLoadOptions"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "خيارات تحميل أرشيف XAR من ملف مضغوط."
type: docs
weight: 142
url: /ar/java/com.aspose.zip/xarloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XarLoadOptions
```

خيارات تحميل أرشيف XAR من ملف مضغوط.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XarLoadOptions()](#XarLoadOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | يضبط علامة الإلغاء المستخدمة لإلغاء عملية الاستخراج. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | يضبط حدثًا يتم إطلاقه عندما يتم استخراج بعض البايتات. |
### XarLoadOptions() {#XarLoadOptions--}
```
public XarLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


يحصل على حدث يتم إطلاقه عندما يتم استخراج بعض البايتات.

```

``````

XarLoadOptions loadOptions = new XarLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / ((XarFileEntry)sender).getLength());
});
XarArchive archive = new XarArchive("archive.xar", loadOptions);
 
```

Event sender is the [XarFileEntry](../../com.aspose.zip/xarfileentry) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel XAR archive extraction after a certain time.

```

``````

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         XarLoadOptions options = new XarLoadOptions();
         options.setCancellationFlag(cf);
         try (XarArchive a = new XarArchive("big.xar", options)) {
             try {
                 ((XarFileEntry) a.getEntries().get(0)).extract("data.bin");
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

XarLoadOptions loadOptions = new XarLoadOptions();
loadOptions.setEntryExtractionProgressed((sender, args) -> {
int percent = (int)((100 * args.getProceededBytes()) / ((XarFileEntry)sender).getLength());
});
XarArchive archive = new XarArchive("archive.xar", loadOptions);
 
```

Event sender is the [XarFileEntry](../../com.aspose.zip/xarfileentry) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

