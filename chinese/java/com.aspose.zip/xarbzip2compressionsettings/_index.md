---
title: "XarBzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "Bzip2 压缩方法的设置。"
type: docs
weight: 137
url: /zh/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Bzip2 压缩方法的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | 初始化 [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) 类的新实例。 |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | 使用默认块大小（相当于 900 千字节）初始化 [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 块大小，以百千字节为单位。 |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


初始化 [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) 类的新实例。

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
