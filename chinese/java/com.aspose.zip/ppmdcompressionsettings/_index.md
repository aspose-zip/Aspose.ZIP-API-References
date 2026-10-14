---
title: "PPMdCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "ZIP 存档中 PPMd 压缩的设置。"
type: docs
weight: 93
url: /zh/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

ZIP 存档中 PPMd 压缩的设置。

PPMd 是由 Dmitry Shkarin 开发的数据压缩算法。该算法基于多阶上下文的预测短语匹配。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | 初始化 [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) 类的新实例。 |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | 初始化 [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) 类的新实例，使用默认的模型阶数和子分配器大小。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | 获取模型的阶数。 |
| [getSuballocatorSize()](#getSuballocatorSize--) | 获取子分配器大小（单位：MB）。 |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


初始化 [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) 类的新实例。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(\"zipFile.zip\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

默认模型阶数为 8，子分配器大小为 50MB。

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


获取模型的阶数。

**Returns:**
int - 模型的阶数
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


获取子分配器大小（单位：MB）。

**Returns:**
int - 子分配器大小（单位：MB）
