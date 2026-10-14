---
title: "DeflateCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "ZIP 存档中 Deflate 压缩的设置。"
type: docs
weight: 59
url: /zh/java/com.aspose.zip/deflatecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class DeflateCompressionSettings extends CompressionSettings
```

ZIP 存档中 Deflate 压缩的设置。

Deflate 是一种无损数据压缩算法，使用 LZ77 算法和哈夫曼编码的组合。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DeflateCompressionSettings()](#DeflateCompressionSettings--) | 初始化一个新的 [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) 类实例。 |
### DeflateCompressionSettings() {#DeflateCompressionSettings--}
```
public DeflateCompressionSettings()
```


初始化一个新的 [DeflateCompressionSettings](../../com.aspose.zip/deflatecompressionsettings) 类实例。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new DeflateCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



