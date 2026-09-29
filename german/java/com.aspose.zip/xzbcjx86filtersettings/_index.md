---
title: "XzBcjX86FilterSettings"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Einstellungen für den xz Bcj X86-Filter."
type: docs
weight: 148
url: /de/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Einstellungen für den xz Bcj X86-Filter.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Initialisiert eine neue Instanz von [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Initialisiert eine neue Instanz von [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Verwenden Sie sie, um ausführbare Dateien und Bibliotheken innerhalb von [XzArchive](../../com.aspose.zip/xzarchive) zu komprimieren.

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



