---
title: "AppleLzmaCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "Apple Archive .aar 文件中 LZMA 压缩的设置。"
type: docs
weight: 23
url: /zh/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Apple Archive（.aar）文件中 LZMA 压缩的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | 初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。 |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | 初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。 |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | 初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。 |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | 使用默认参数初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 获取压缩前每个数据块的大小。 |
| [getDictionarySize()](#getDictionarySize--) | 获取用于压缩的字典大小。 |
| [getFastBytes()](#getFastBytes--) | 获取用于压缩的快速字节数。 |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 压缩前每个数据块的大小。 |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 压缩前每个数据块的大小。 |
| dictionarySize | int | 用于压缩的字典大小。 |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 压缩前每个数据块的大小。 |
| dictionarySize | int | 用于压缩的字典大小。 |
| fastBytes | int | 用于压缩的快速字节数。 |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


使用默认参数初始化 [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) 类的新实例。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


获取压缩前每个数据块的大小。

值：默认值为 4 MiB。

**Returns:**
int - 压缩前每个数据块的大小。
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


获取用于压缩的字典大小。

值：默认值为 8 MiB。

**Returns:**
int - 用于压缩的字典大小。
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


获取用于压缩的快速字节数。

值：默认值为 32。

**Returns:**
int - 用于压缩的快速字节数。
