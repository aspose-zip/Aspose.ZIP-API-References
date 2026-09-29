---
title: "AppleLz4CompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "Apple Archive .aar 文件中 LZ4 压缩的设置。"
type: docs
weight: 21
url: /zh/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Apple Archive（.aar）文件中 LZ4 压缩的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | 初始化 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 类的新实例。 |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | 使用默认参数初始化 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 获取每个压缩的 `pbz4`/`bv41` 块的大小。 |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


初始化 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 每个压缩的 `pbz4`/`bv41` 块的大小。 |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


使用默认参数初始化 [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) 类的新实例。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


获取每个压缩的 `pbz4`/`bv41` 块的大小。

值：默认值为 4 MiB。

**Returns:**
int - 每个压缩的 `pbz4`/`bv41` 块的大小。
