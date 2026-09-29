---
title: "SevenZipBZip2CompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "7z 存档中 BZip2 压缩方法的设置。"
type: docs
weight: 109
url: /zh/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

7z 存档中 BZip2 压缩方法的设置。

Bzip2 使用 Burrows-Wheeler 块排序文本压缩算法和哈夫曼编码来压缩文件。

查看更多: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | 初始化 [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 类的新实例。 |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | 使用默认块大小（等于 9 百千字节）初始化 [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 块大小，以百千字节为单位。 |
| [getMethod()](#getMethod--) | 获取压缩或解压缩方法。 |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


初始化 [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| blockSize | int | 块大小（以百千字节为单位） |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


使用默认块大小（等于 9 百千字节）初始化 [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) 类的新实例。

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


块大小，以百千字节为单位。

**Returns:**
int - 块大小，以百千字节为单位
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


获取压缩或解压缩方法。

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
