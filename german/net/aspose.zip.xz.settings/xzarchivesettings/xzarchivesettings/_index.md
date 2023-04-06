---
title: XzArchiveSettings.XzArchiveSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: XzArchiveSettings constructeur. Initialisiert eine neue Instanz vonXzArchiveSettings Klasse mit einfacher LZMA2Komprimierung.
type: docs
weight: 10
url: /de/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Initialisiert eine neue Instanz von[`XzArchiveSettings`](../) Klasse mit einfacher LZMA2-Komprimierung.

```csharp
public XzArchiveSettings()
```

### Bemerkungen

Standard-Wörterbuch in LZMA2-Filtergröße ist gleich 16 Megabyte, Standard-Blockgröße ist gleich 64 Megabyte, Standard-Prüfsummentyp ist CRC32.

### Siehe auch

* class [XzArchiveSettings](../)
* namensraum [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* Montage [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Initialisiert eine neue Instanz von[`XzArchiveSettings`](../) Klasse mit benutzerdefinierten Parametern.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filters | XzFilterSettings[] | Filter (Kompressoren) werden nacheinander angewendet, um zu erstellen[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . Es kann entweder Single sein[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) oder ein Paar[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) Und[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Größe xz Archivblock. |
| checkType | XzCheckType | Art der Prüfsummenberechnung für unkomprimierte Daten. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* ist negativ. |
| ArgumentNullException | *filters* ist Null |
| ArgumentException | *filters* hat weniger als einen oder mehr als zwei Filter oder der letzte Filter nicht[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Beispiele

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Siehe auch

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* namensraum [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* Montage [Aspose.Zip](../../../)


