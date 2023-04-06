---
title: CpioArchive.SaveGzipped
second_title: Aspose.ZIP für .NET-API-Referenz
description: CpioArchive methode. Speichert das Archiv mit gzipKomprimierung im Stream.
type: docs
weight: 90
url: /de/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

Speichert das Archiv mit gzip-Komprimierung im Stream.

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| output | Stream | Zielstrom. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist Null. |
| ArgumentException | *output* ist nicht beschreibbar. |

### Bemerkungen

*output*muss beschreibbar sein.

### Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

Speichert das Archiv in der Datei nach Pfad mit gzip-Komprimierung.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| cpioFormat | CpioFormat | Definiert das cpio-Header-Format. |

### Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### Siehe auch

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namensraum [Aspose.Zip.Cpio](../../cpioarchive/)
* Montage [Aspose.Zip](../../../)


