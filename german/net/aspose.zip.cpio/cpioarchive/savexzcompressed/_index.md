---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP für .NET-API-Referenz
description: CpioArchive methode. Speichert das Archiv mit xzKomprimierung im Stream.
type: docs
weight: 100
url: /de/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Speichert das Archiv mit xz-Komprimierung im Stream.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| output | Stream | Zielstrom. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |
| settings | XzArchiveSettings | Einstellungssatz für bestimmte xz-Archive: Wörterbuchgröße, Blockgröße, Überprüfungstyp. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist Null. |
| ArgumentException | *output* ist nicht beschreibbar. |

### Bemerkungen

*output*Der Stream muss beschreibbar sein.

### Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Speichert das Archiv Pfad für Pfad mit xz-Komprimierung.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |
| settings | XzArchiveSettings | Einstellungssatz für bestimmte xz-Archive: Wörterbuchgröße, Blockgröße, Überprüfungstyp. |

### Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)


