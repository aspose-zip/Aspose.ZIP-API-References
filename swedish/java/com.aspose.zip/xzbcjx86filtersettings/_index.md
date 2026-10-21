---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Inställningar för xz Bcj X86-filter."
type: docs
weight: 148
url: /sv/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Inställningar för xz Bcj X86-filter.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Initierar en ny instans av [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Initierar en ny instans av [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Använd den för att komprimera körbara filer och bibliotek inom [XzArchive](../../com.aspose.zip/xzarchive).

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



