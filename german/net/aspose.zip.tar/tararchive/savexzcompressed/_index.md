---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarArchive methode. Speichert das Archiv mit xzKomprimierung im Stream.
type: docs
weight: 150
url: /de/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Speichert das Archiv mit xz-Komprimierung im Stream.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| output | Stream | Zielstrom. |
| format | Nullable`1 | Definiert das tar-Header-Format. Nullwerte werden nach Möglichkeit als UStar behandelt. |
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
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Speichert das Archiv Pfad für Pfad mit xz-Komprimierung.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| format | Nullable`1 | Definiert das tar-Header-Format. Nullwerte werden nach Möglichkeit als UStar behandelt. |
| settings | XzArchiveSettings | Einstellungssatz für bestimmte xz-Archive: Wörterbuchgröße, Blockgröße, Überprüfungstyp. |

### Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)


