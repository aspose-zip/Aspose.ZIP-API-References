---
title: "XzBcjX86FilterSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk filter xz Bcj X86."
type: docs
weight: 148
url: /id/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Pengaturan untuk filter xz Bcj X86.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Menginisialisasi sebuah instance baru dari [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Menginisialisasi sebuah instance baru dari [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Gunakan untuk mengompresi file eksekusi dan pustaka dalam [XzArchive](../../com.aspose.zip/xzarchive).

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



