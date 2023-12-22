---
title: ArchiveSaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving a zip archive.
type: docs
weight: 20
url: /java/com.aspose.zip/archivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class ArchiveSaveOptions
```

Options for saving a zip archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArchiveSaveOptions()](#ArchiveSaveOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Gets optional comment for the Zip file. |
| [getEncoding()](#getEncoding--) | Gets encoding for converting file names and other strings to bytes. |
| [getEventsBag()](#getEventsBag--) | Gets container of events raising on archive saving. |
| [getParallelOptions()](#getParallelOptions--) | Gets settings for parallel compression. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Sets optional comment for the Zip file. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets encoding for converting file names and other strings to bytes. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Sets container of events raising on archive saving. |
| [setParallelOptions(ParallelOptions value)](#setParallelOptions-com.aspose.zip.ParallelOptions-) | Sets settings for parallel compression. |
### ArchiveSaveOptions() {#ArchiveSaveOptions--}
```
public ArchiveSaveOptions()
```


### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Gets optional comment for the Zip file.

**Returns:**
java.lang.String - optional comment for the Zip file.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Gets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Returns:**
java.nio.charset.Charset - encoding for converting file names and other strings to bytes.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Gets container of events raising on archive saving.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getParallelOptions() {#getParallelOptions--}
```
public final ParallelOptions getParallelOptions()
```


Gets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Returns:**
[ParallelOptions](../../com.aspose.zip/paralleloptions) - settings for parallel compression.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Sets optional comment for the Zip file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | optional comment for the Zip file. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Sets encoding for converting file names and other strings to bytes.

If not set, code page 437 will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.nio.charset.Charset | encoding for converting file names and other strings to bytes. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Sets container of events raising on archive saving.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | container of events raising on archive saving. |

### setParallelOptions(ParallelOptions value) {#setParallelOptions-com.aspose.zip.ParallelOptions-}
```
public final void setParallelOptions(ParallelOptions value)
```


Sets settings for parallel compression.

Assign it if you want to utilize several CPU cores while compressing several archive entries.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ParallelOptions](../../com.aspose.zip/paralleloptions) | settings for parallel compression. |

