---
title: "XzBcjX86FilterSettings"
second_title: "مرجع API لـ Aspose.ZIP للـ Java"
description: "إعدادات مرشح xz Bcj X86."
type: docs
weight: 148
url: /ar/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

إعدادات مرشح xz Bcj X86.
## المُنشئات

| مُنشئ | الوصف |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | ينشئ مثيلاً جديداً من [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


ينشئ مثيلاً جديداً من [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). استخدمه لضغط الملفات التنفيذية والمكتبات داخل [XzArchive](../../com.aspose.zip/xzarchive).

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save("archive.xz");
}
 
```



