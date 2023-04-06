---
title: TarArchive.SaveGzipped
second_title: Aspose.ZIP für .NET-API-Referenz
description: TarArchive methode. Speichert das Archiv mit gzipKomprimierung im Stream.
type: docs
weight: 130
url: /de/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Speichert das Archiv mit gzip-Komprimierung im Stream.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| output | Stream | Zielstrom. |
| format | Nullable`1 | Definiert das tar-Header-Format. Nullwerte werden nach Möglichkeit als UStar behandelt. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | *output* ist Null. |
| ArgumentException | *output* ist nicht beschreibbar. |

### Bemerkungen

*output*muss beschreibbar sein.

### Beispiele

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Speichert das Archiv in der Datei nach Pfad mit gzip-Komprimierung.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| path | String | Der Pfad des zu erstellenden Archivs. Wenn der angegebene Dateiname auf eine vorhandene Datei verweist, wird diese überschrieben. |
| format | Nullable`1 | Definiert das tar-Header-Format. Nullwerte werden nach Möglichkeit als UStar behandelt. |

### Beispiele

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### Siehe auch

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namensraum [Aspose.Zip.Tar](../../tararchive/)
* Montage [Aspose.Zip](../../../)


