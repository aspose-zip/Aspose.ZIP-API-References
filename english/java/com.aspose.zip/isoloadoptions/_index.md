---
title: IsoLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which  is loaded from a compressed file.
type: docs
weight: 47
url: /java/com.aspose.zip/isoloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class IsoLoadOptions
```

Options with which [IsoArchive](../../com.aspose.zip/isoarchive) is loaded from a compressed file. Contains event raised on extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [IsoLoadOptions()](#IsoLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
| [setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when some bytes have been extracted. |
### IsoLoadOptions() {#IsoLoadOptions--}
```
public IsoLoadOptions()
```


### getEntryExtractionProgressed() {#getEntryExtractionProgressed--}
```
public final Event<ProgressEventArgs> getEntryExtractionProgressed()
```


Gets an event that is raised when some bytes have been extracted.

```

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
### setEntryExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setEntryExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setEntryExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when some bytes have been extracted.

```

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

