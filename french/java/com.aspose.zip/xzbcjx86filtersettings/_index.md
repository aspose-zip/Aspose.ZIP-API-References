---
title: "XzBcjX86FilterSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour le filtre xz Bcj X86."
type: docs
weight: 148
url: /fr/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Paramètres pour le filtre xz Bcj X86.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Initialise une nouvelle instance de la [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Initialise une nouvelle instance de la [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Utilisez‑la pour compresser les fichiers exécutables et les bibliothèques au sein de [XzArchive](../../com.aspose.zip/xzarchive).

```

``````

XzLZMA2FilterSettings lzma2 = new XzLZMA2FilterSettings(5242880);
XzBcjX86FilterSettings bcj = new XzBcjX86FilterSettings();
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {bcj,lzma2}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource(\"data.bin\");
archive.save(\"archive.xz\");
}
 
```



