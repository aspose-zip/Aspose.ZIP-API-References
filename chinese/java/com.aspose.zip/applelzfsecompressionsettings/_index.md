---
title: "AppleLzfseCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "Apple Archive .aar 文件中 LZFSE 压缩的设置。"
type: docs
weight: 22
url: /zh/java/com.aspose.zip/applelzfsecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzfseCompressionSettings extends AppleCompressionSettings
```

Apple Archive（.aar）文件中 LZFSE 压缩的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AppleLzfseCompressionSettings(int blockSize)](#AppleLzfseCompressionSettings-int-) | 初始化 [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) 类的新实例。 |
| [AppleLzfseCompressionSettings()](#AppleLzfseCompressionSettings--) | 使用默认参数初始化 [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 获取压缩前每个数据块的大小。 |
### AppleLzfseCompressionSettings(int blockSize) {#AppleLzfseCompressionSettings-int-}
```
public AppleLzfseCompressionSettings(int blockSize)
```


初始化 [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 压缩前每个数据块的大小。 |

### AppleLzfseCompressionSettings() {#AppleLzfseCompressionSettings--}
```
public AppleLzfseCompressionSettings()
```


使用默认参数初始化 [AppleLzfseCompressionSettings](../../com.aspose.zip/applelzfsecompressionsettings) 类的新实例。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


获取压缩前每个数据块的大小。

值：默认值为 4 MiB。

**Returns:**
int - 压缩前每个数据块的大小。
