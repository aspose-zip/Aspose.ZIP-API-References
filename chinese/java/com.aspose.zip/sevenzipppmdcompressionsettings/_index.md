---
title: "SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "7z 存档中 PPMd 压缩方法的设置。"
type: docs
weight: 117
url: /zh/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

7z 存档中 PPMd 压缩方法的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | 实例化 7z 存档中 PPMd 压缩方法的设置。 |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | 实例化 7z 存档中 PPMd 压缩方法的设置，使用默认模型顺序和子分配器大小。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | 获取最大阶。 |
| [getMethod()](#getMethod--) | 获取压缩或解压缩方法。 |
| [getSuballocatorSize()](#getSuballocatorSize--) | 获取子分配器大小（单位：MB）。 |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


实例化 7z 存档中 PPMd 压缩方法的设置。

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(\"zipFile.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

默认模型阶为 6，子分配器大小为 16MB。

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


获取最大阶。

**Returns:**
byte - 最大阶
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


获取压缩或解压缩方法。

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


获取子分配器大小（单位：MB）。

**Returns:**
int - 子分配器大小（单位：MB）
