---
title: Bzip2LoadOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for loading .
type: docs
weight: 23
url: /java/com.aspose.zip/bzip2loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class Bzip2LoadOptions
```

Options for loading [Bzip2Archive](../../com.aspose.zip/bzip2archive). Contains event raised on extraction.
## Constructors

| Constructor | Description |
| --- | --- |
| [Bzip2LoadOptions()](#Bzip2LoadOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getExtractionProgressed()](#getExtractionProgressed--) | Gets an event that is raised when some bytes have been extracted. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Sets an event that is raised when some bytes have been extracted. |
### Bzip2LoadOptions() {#Bzip2LoadOptions--}
```
public Bzip2LoadOptions()
```


### getExtractionProgressed() {#getExtractionProgressed--}
```
public Event<ProgressEventArgs> getExtractionProgressed()
```


Gets an event that is raised when some bytes have been extracted.

```

     int[] percent = { 0 };
     long originalFileLength = 10_000_000;

     Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
     loadOptions.setExtractionProgressed((sender, args) -> {
         percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
     });
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when some bytes have been extracted
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when some bytes have been extracted.

```

     int[] percent = { 0 };
     long originalFileLength = 10_000_000;

     Bzip2LoadOptions loadOptions = new Bzip2LoadOptions();
     loadOptions.setExtractionProgressed((sender, args) -> {
         percent[0] = (int)((100 * (double)args.getProceededBytes()) / originalFileLength);
     });
 
```

Event sender is the [Bzip2Archive](../../com.aspose.zip/bzip2archive) instance which extraction is progressed. The `ProgressEventArgs.getProceededBytes()`([ProgressEventArgs.getProceededBytes()](../../com.aspose.zip/progresseventargs\#getProceededBytes--)) is the number of bytes after extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when some bytes have been extracted |
