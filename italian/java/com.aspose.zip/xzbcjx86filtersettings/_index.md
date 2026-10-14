---
title: "XzBcjX86FilterSettings"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Impostazioni per il filtro xz Bcj X86."
type: docs
weight: 148
url: /it/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Impostazioni per il filtro xz Bcj X86.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Inizializza una nuova istanza di [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Inizializza una nuova istanza di [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Usalo per comprimere file eseguibili e librerie all'interno di [XzArchive](../../com.aspose.zip/xzarchive).

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



