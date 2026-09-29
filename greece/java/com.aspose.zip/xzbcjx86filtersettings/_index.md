---
title: "XzBcjX86FilterSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για το φίλτρο xz Bcj X86."
type: docs
weight: 148
url: /el/java/com.aspose.zip/xzbcjx86filtersettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XzFilterSettings](../../com.aspose.zip/xzfiltersettings)
```
public final class XzBcjX86FilterSettings extends XzFilterSettings
```

Ρυθμίσεις για το φίλτρο xz Bcj X86.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XzBcjX86FilterSettings()](#XzBcjX86FilterSettings--) | Αρχικοποιεί μια νέα παρουσία του [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). |
### XzBcjX86FilterSettings() {#XzBcjX86FilterSettings--}
```
public XzBcjX86FilterSettings()
```


Αρχικοποιεί μια νέα παρουσία του [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings). Χρησιμοποιήστε το για να συμπιέσετε εκτελέσιμα αρχεία και βιβλιοθήκες εντός του [XzArchive](../../com.aspose.zip/xzarchive).

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



