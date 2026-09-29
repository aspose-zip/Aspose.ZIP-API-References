---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Instellingen voor xz Bcj X86-filter."
type: docs
weight: 148
url: /nl/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Instellingen voor xz Bcj X86-filter.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Initialiseert een nieuw exemplaar van de [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Initialiseert een nieuw exemplaar van de [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Gebruik het om uitvoerbare bestanden en bibliotheken te comprimeren binnen [XzArchive](../../com.aspose.zip/xzarchive).

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



