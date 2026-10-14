---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP for Java API 参考"
description: "xz Bcj X86 过滤器的设置。"
type: docs
weight: 148
url: /zh/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

xz Bcj X86 过滤器的设置。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | 初始化 [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) 的新实例。 |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


初始化 [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) 的新实例。用于压缩可执行文件和位于 [XzArchive](../../com.aspose.zip/xzarchive) 中的库。

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save("archive.xz");
}
 
```



