---
title: "XzCompressionSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "ZIP 存档中 Xz 压缩的设置。"
type: docs
weight: 149
url: /zh/java/com.aspose.zip/xzcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class XzCompressionSettings extends CompressionSettings
```

ZIP 存档中 Xz 压缩的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XzCompressionSettings()](#XzCompressionSettings--) | 初始化 [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) 类的新实例。 |
### XzCompressionSettings() {#XzCompressionSettings--}
```
public XzCompressionSettings()
```


初始化 [XzCompressionSettings](../../com.aspose.zip/xzcompressionsettings) 类的新实例。

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new XzCompressionSettings()))) {
archive.createEntry("data.bin", "data.bin");
archive.save("archive.zip");
}
 
```



