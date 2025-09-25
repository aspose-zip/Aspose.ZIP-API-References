---
title: XarLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which XAR archive is loaded from a compressed file.
type: docs
weight: 119
url: /java/com.aspose.zip/xarloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XarLoadOptions
```

Options with which XAR archive is loaded from a compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [XarLoadOptions()](#XarLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when some bytes have been extracted. |
### XarLoadOptions() {#XarLoadOptions--}
```
public XarLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Gets an event that is raised when some bytes have been extracted.

```

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

Cancellation mostly results in some data not being extracted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | a cancellation flag used to cancel the extraction operation. |

### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when some bytes have been extracted.

```

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

