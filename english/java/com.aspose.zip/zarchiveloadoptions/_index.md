---
title: ZArchiveLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which  is loaded from a compressed file.
type: docs
weight: 137
url: /java/com.aspose.zip/zarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZArchiveLoadOptions
```

Options with which [ZArchive](../../com.aspose.zip/zarchive) is loaded from a compressed file. Contains event raised on extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [ZArchiveLoadOptions()](#ZArchiveLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Sets a cancellation flag used to cancel the extraction operation. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when some bytes have been extracted. |
### ZArchiveLoadOptions() {#ZArchiveLoadOptions--}
```
public ZArchiveLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Gets an event that is raised when some bytes have been extracted.

```

     long length = 10_000_000;
     ZArchiveLoadOptions loadOptions = new ZArchiveLoadOptions();
     loadOptions.setExtractionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / length);
     });
     ZArchive archive = new ZArchive("archive.z", loadOptions);
 
```

Event sender is the [ZArchive](../../com.aspose.zip/zarchive) instance which extraction is progressed.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Sets a cancellation flag used to cancel the extraction operation.

Cancel Z archive extraction after a certain time.

```

     try (CancellationFlag cf = new CancellationFlag()) {
         cf.cancelAfter(TimeUnit.SECONDS.toMillis(60));
         ZArchiveLoadOptions options = new ZArchiveLoadOptions();
         options.setCancellationFlag(cf);
         try (ZArchive a = new ZArchive("big.z", options)) {
             try {
                 a.extract("data.bin");
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

### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when some bytes have been extracted.

```

     long length = 10_000_000;
     ZArchiveLoadOptions loadOptions = new ZArchiveLoadOptions();
     loadOptions.setExtractionProgressed((sender, args) -> {
         int percent = (int)((100 * args.getProceededBytes()) / length);
     });
     ZArchive archive = new ZArchive("archive.z", loadOptions);
 
```

Event sender is the [ZArchive](../../com.aspose.zip/zarchive) instance which extraction is progressed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |

