---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "xz Bcj X86 filtresi için ayarlar."
type: docs
weight: 148
url: /tr/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

xz Bcj X86 filtresi için ayarlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Yeni bir [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) örneği oluşturur. |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Yeni bir [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) örneği oluşturur. Yürütülebilir dosyaları ve kütüphaneleri [XzArchive](../../com.aspose.zip/xzarchive) içinde sıkıştırmak için kullanın.

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



