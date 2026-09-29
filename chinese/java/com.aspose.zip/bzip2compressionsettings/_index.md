---
title: "Bzip2CompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "ZIP 存档中 Bzip2 压缩的设置。"
type: docs
weight: 41
url: /zh/java/com.aspose.zip/bzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class Bzip2CompressionSettings extends CompressionSettings
```

ZIP 存档中 Bzip2 压缩的设置。

bzip2 使用 Burrows-Wheeler 块排序文本压缩算法和哈夫曼编码来压缩文件。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Bzip2CompressionSettings(int blockSize)](#Bzip2CompressionSettings-int-) | 初始化 [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) 类的新实例。 |
| [Bzip2CompressionSettings()](#Bzip2CompressionSettings--) | 使用默认块大小（相当于 9 百千字节）初始化 [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | 块大小，以百千字节为单位。 |
### Bzip2CompressionSettings(int blockSize) {#Bzip2CompressionSettings-int-}
```
public Bzip2CompressionSettings(int blockSize)
```


初始化 [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) 类的新实例。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1)))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | Block size in hundreds of kilobytes. |

### Bzip2CompressionSettings() {#Bzip2CompressionSettings--}
```
public Bzip2CompressionSettings()
```


Initializes a new instance of the [Bzip2CompressionSettings](../../com.aspose.zip/bzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save(zipFile);
     }
 
```



### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


块大小，以百千字节为单位。

**Returns:**
int - 块大小，以百千字节为单位
