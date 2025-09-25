---
title: SplitSevenZipArchiveSaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving a multi-volume 7-zip archive.
type: docs
weight: 100
url: /java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Options for saving a multi-volume 7-zip archive.
## Constructors

| Constructor | Description |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Instantiates settings for saving a multi-volume 7z archive. |
## Methods

| Method | Description |
| --- | --- |
| [getFileName()](#getFileName--) | Gets the name of segments without extension. |
| [getSegmentSize()](#getSegmentSize--) | Gets the size of the segment. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Instantiates settings for saving a multi-volume 7z archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | name for volumes. May be with or without .7z extension.

Names of files will be as follows: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
| segmentSize | long | size of volume.

Some volumes may be less than `segmentSize`. In most cases, the last segment will be less but rarely regular segments might be too. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Gets the name of segments without extension.

**Returns:**
java.lang.String - the name of segments without extension
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Gets the size of the segment.

**Returns:**
long - the size of the segment.
