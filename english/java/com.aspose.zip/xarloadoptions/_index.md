---
title: XarLoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options with which archive is loaded from compressed file.
type: docs
weight: 102
url: /java/com.aspose.zip/xarloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class XarLoadOptions
```

Options with which archive is loaded from compressed file.
## Constructors

| Constructor | Description |
| --- | --- |
| [XarLoadOptions()](#XarLoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getEntryExtractionProgressed()](#getEntryExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
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

