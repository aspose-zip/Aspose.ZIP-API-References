---
title: CabEntrySettings
second_title: Aspose.ZIP for Java API Reference
description: Settings that control how a CAB entry is written.
type: docs
weight: 31
url: /java/com.aspose.zip/cabentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class CabEntrySettings
```

Settings that control how a CAB entry is written.
## Constructors

| Constructor | Description |
| --- | --- |
| [CabEntrySettings(CabCompressionSettings compressionSettings)](#CabEntrySettings-com.aspose.zip.CabCompressionSettings-) | Initializes settings with a specific compression profile. |
| [CabEntrySettings()](#CabEntrySettings--) | Initializes settings with default MSZip compression. |
## Methods

| Method | Description |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | Gets the compression configuration applied to the entry. |
### CabEntrySettings(CabCompressionSettings compressionSettings) {#CabEntrySettings-com.aspose.zip.CabCompressionSettings-}
```
public CabEntrySettings(CabCompressionSettings compressionSettings)
```


Initializes settings with a specific compression profile.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compressionSettings | [CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) | Compression settings to use.

Can be one of these: |

### CabEntrySettings() {#CabEntrySettings--}
```
public CabEntrySettings()
```


Initializes settings with default MSZip compression.

### getCompressionSettings() {#getCompressionSettings--}
```
public final CabCompressionSettings getCompressionSettings()
```


Gets the compression configuration applied to the entry.

Can be one of these:

 *  

**Returns:**
[CabCompressionSettings](../../com.aspose.zip/cabcompressionsettings) - the compression configuration applied to the entry.
