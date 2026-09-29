---
title: "StoreCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "ZIP 存档中 Store 压缩的设置。"
type: docs
weight: 124
url: /zh/java/com.aspose.zip/storecompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class StoreCompressionSettings extends CompressionSettings
```

ZIP 存档中 Store 压缩的设置。

此方法按原样存储原始数据。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [StoreCompressionSettings()](#StoreCompressionSettings--) | 初始化 [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) 类的新实例。 |
### StoreCompressionSettings() {#StoreCompressionSettings--}
```
public StoreCompressionSettings()
```


初始化 [StoreCompressionSettings](../../com.aspose.zip/storecompressionsettings) 类的新实例。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new StoreCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save(zipFile);
}
 
```



