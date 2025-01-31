---
title: ZstandardLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which  is loaded from compressed file.
type: docs
weight: 119
url: /java/com.aspose.zip/zstandardloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class ZstandardLoadOptions
```

Options with which [ZstandardArchive](../../com.aspose.zip/zstandardarchive) is loaded from compressed file. Contains event raised on extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [ZstandardLoadOptions()](#ZstandardLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when some bytes have been extracted. |
### ZstandardLoadOptions() {#ZstandardLoadOptions--}
```
public ZstandardLoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Gets an event that is raised when some bytes have been extracted.

```

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
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when some bytes have been extracted.

```

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

