---
title: "AppleZlibCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "Apple Archive .aar 文件中 Zlib 压缩的设置。"
type: docs
weight: 25
url: /zh/java/com.aspose.zip/applezlibcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleZlibCompressionSettings extends AppleCompressionSettings
```

Apple Archive（.aar）文件中 Zlib 压缩的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AppleZlibCompressionSettings(int blockSize)](#AppleZlibCompressionSettings-int-) | 初始化 [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) 类的新实例。 |
| [AppleZlibCompressionSettings()](#AppleZlibCompressionSettings--) | 使用默认参数初始化 [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 获取压缩前每个数据块的大小。 |
### AppleZlibCompressionSettings(int blockSize) {#AppleZlibCompressionSettings-int-}
```
public AppleZlibCompressionSettings(int blockSize)
```


初始化 [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 压缩前每个数据块的大小。 |

### AppleZlibCompressionSettings() {#AppleZlibCompressionSettings--}
```
public AppleZlibCompressionSettings()
```


使用默认参数初始化 [AppleZlibCompressionSettings](../../com.aspose.zip/applezlibcompressionsettings) 类的新实例。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


获取压缩前每个数据块的大小。

值：默认值为 4 MiB。

**Returns:**
int - 压缩前每个数据块的大小。
