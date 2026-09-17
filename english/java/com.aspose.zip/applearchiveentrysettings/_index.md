---
title: AppleArchiveEntrySettings
second_title: Aspose.ZIP for Java API Reference
description: Settings used to compose entries inside .
type: docs
weight: 18
url: /java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

Settings used to compose entries inside [AppleArchive](../../com.aspose.zip/applearchive).
## Constructors

| Constructor | Description |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | Initializes a new instance of the [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) class. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Gets compression settings applied to the composed Apple Archive payload. |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | Gets a value indicating whether CRC32 checksum fields are included for composed file entries. |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | Sets a value indicating whether CRC32 checksum fields are included for composed file entries. |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


Initializes a new instance of the [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | Compression settings applied to the composed Apple Archive payload. |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


Gets compression settings applied to the composed Apple Archive payload.

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


Gets a value indicating whether CRC32 checksum fields are included for composed file entries.

**Returns:**
boolean - a value indicating whether CRC32 checksum fields are included for composed file entries.
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


Sets a value indicating whether CRC32 checksum fields are included for composed file entries.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether CRC32 checksum fields are included for composed file entries. |

