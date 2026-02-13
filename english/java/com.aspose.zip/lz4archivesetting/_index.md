---
title: Lz4ArchiveSetting
second_title: Aspose.ZIP for Java API Reference
description: Settings for LZ4 archive composition.
type: docs
weight: 64
url: /java/com.aspose.zip/lz4archivesetting/
---

**Inheritance:**
java.lang.Object
```
public class Lz4ArchiveSetting
```

Settings for LZ4 archive composition.
## Constructors

| Constructor | Description |
| --- | --- |
| [Lz4ArchiveSetting()](#Lz4ArchiveSetting--) | Initializes a new instance of the [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) with default parameters. |
## Methods

| Method | Description |
| --- | --- |
| [getIncludeBlockChecksum()](#getIncludeBlockChecksum--) | Gets a value indicating whether to include compressed xxh32 hash at the end of compressed block. |
| [getIncludeContentChecksum()](#getIncludeContentChecksum--) | Gets a value indicating whether to include content xxh32 hash at the end of LZ4 archive. |
| [getIncludeContentSize()](#getIncludeContentSize--) | Gets a value indicating whether to include the content size in the frame. |
| [setIncludeBlockChecksum(boolean value)](#setIncludeBlockChecksum-boolean-) | Sets a value indicating whether to include compressed xxh32 hash at the end of compressed block. |
| [setIncludeContentChecksum(boolean value)](#setIncludeContentChecksum-boolean-) | Sets a value indicating whether to include content xxh32 hash at the end of LZ4 archive. |
| [setIncludeContentSize(boolean value)](#setIncludeContentSize-boolean-) | Sets a value indicating whether to include the content size in the frame. |
### Lz4ArchiveSetting() {#Lz4ArchiveSetting--}
```
public Lz4ArchiveSetting()
```


Initializes a new instance of the [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) with default parameters.

### getIncludeBlockChecksum() {#getIncludeBlockChecksum--}
```
public final boolean getIncludeBlockChecksum()
```


Gets a value indicating whether to include compressed xxh32 hash at the end of compressed block.

Default is false.

**Returns:**
boolean - a value indicating whether to include compressed xxh32 hash at the end of compressed block.
### getIncludeContentChecksum() {#getIncludeContentChecksum--}
```
public final boolean getIncludeContentChecksum()
```


Gets a value indicating whether to include content xxh32 hash at the end of LZ4 archive.

Default is true.

**Returns:**
boolean - a value indicating whether to include content xxh32 hash at the end of LZ4 archive.
### getIncludeContentSize() {#getIncludeContentSize--}
```
public final boolean getIncludeContentSize()
```


Gets a value indicating whether to include the content size in the frame.

Default is false. Applied when the source stream is seekable.

**Returns:**
boolean - a value indicating whether to include the content size in the frame.
### setIncludeBlockChecksum(boolean value) {#setIncludeBlockChecksum-boolean-}
```
public final void setIncludeBlockChecksum(boolean value)
```


Sets a value indicating whether to include compressed xxh32 hash at the end of compressed block.

Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to include compressed xxh32 hash at the end of compressed block. |

### setIncludeContentChecksum(boolean value) {#setIncludeContentChecksum-boolean-}
```
public final void setIncludeContentChecksum(boolean value)
```


Sets a value indicating whether to include content xxh32 hash at the end of LZ4 archive.

Default is true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to include content xxh32 hash at the end of LZ4 archive. |

### setIncludeContentSize(boolean value) {#setIncludeContentSize-boolean-}
```
public final void setIncludeContentSize(boolean value)
```


Sets a value indicating whether to include the content size in the frame.

Default is false. Applied when the source stream is seekable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether to include the content size in the frame. |

