---
title: SplitArchiveSaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving a multi-volume zip archive.
type: docs
weight: 57
url: /java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Options for saving a multi-volume zip archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Instantiates settings for saving a multi-volume zip archive. |
## Methods

| Method | Description |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Gets optional comment for the Zip file. |
| [getEncoding()](#getEncoding--) | Gets encoding for converting file names and other strings to bytes. |
| [getFileName()](#getFileName--) | Gets the name of segments without extension. |
| [getSegmentSize()](#getSegmentSize--) | Gets the size of segment. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Sets optional comment for the Zip file. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Sets encoding for converting file names and other strings to bytes. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Instantiates settings for saving a multi-volume zip archive.

Some volumes may be less than `segmentSize`. In most cases the last segment will be less but rarely regular segments might be too.

Names of files will be as follows: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | Name for volumes. May be with or without .zip extension. |
| segmentSize | long | Size of volume. |

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
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Gets the name of segments without extension.

**Returns:**
java.lang.String - the name of segments without extension.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Gets the size of segment.

**Returns:**
long - the size of segment.
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

