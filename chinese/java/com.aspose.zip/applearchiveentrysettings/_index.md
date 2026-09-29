---
title: "AppleArchiveEntrySettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "用于在内部组合条目的设置。"
type: docs
weight: 18
url: /zh/java/com.aspose.zip/applearchiveentrysettings/
---

**Inheritance:**
java.lang.Object
```
public class AppleArchiveEntrySettings
```

用于在 [AppleArchive](../../com.aspose.zip/applearchive) 中组合条目的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)](#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-) | 初始化 [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getCompressionSettings()](#getCompressionSettings--) | 获取应用于已组合 Apple Archive 负载的压缩设置。 |
| [getIncludeCrc32Checksum()](#getIncludeCrc32Checksum--) | 获取一个值，指示是否为已组合的文件条目包含 CRC32 校验和字段。 |
| [setIncludeCrc32Checksum(boolean value)](#setIncludeCrc32Checksum-boolean-) | 设置一个值，指示是否为已组合的文件条目包含 CRC32 校验和字段。 |
### AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings) {#AppleArchiveEntrySettings-com.aspose.zip.AppleCompressionSettings-}
```
public AppleArchiveEntrySettings(AppleCompressionSettings compressionSettings)
```


初始化 [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| compressionSettings | [AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) | 应用于已组合 Apple Archive 负载的压缩设置。 |

### getCompressionSettings() {#getCompressionSettings--}
```
public final AppleCompressionSettings getCompressionSettings()
```


获取应用于已组合 Apple Archive 负载的压缩设置。

**Returns:**
[AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings) - compression settings applied to the composed Apple Archive payload.
### getIncludeCrc32Checksum() {#getIncludeCrc32Checksum--}
```
public final boolean getIncludeCrc32Checksum()
```


获取一个值，指示是否为已组合的文件条目包含 CRC32 校验和字段。

**Returns:**
boolean - 一个值，指示是否为已组合的文件条目包含 CRC32 校验和字段。
### setIncludeCrc32Checksum(boolean value) {#setIncludeCrc32Checksum-boolean-}
```
public final void setIncludeCrc32Checksum(boolean value)
```


设置一个值，指示是否为已组合的文件条目包含 CRC32 校验和字段。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | 布尔 | 一个值，指示是否为已组合的文件条目包含 CRC32 校验和字段。 |

