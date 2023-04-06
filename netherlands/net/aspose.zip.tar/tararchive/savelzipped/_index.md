---
title: TarArchive.SaveLzipped
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Slaat archief op in de stream met lzipcompressie.
type: docs
weight: 140
url: /nl/net/aspose.zip.tar/tararchive/savelzipped/
---
## SaveLzipped(Stream, TarFormat?) {#savelzipped}

Slaat archief op in de stream met lzip-compressie.

```csharp
public void SaveLzipped(Stream output, TarFormat? format = default)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| output | Stream | Bestemmingsstroom. |
| format | Nullable`1 | Definieert het formaat van de tar-koptekst. Null-waarde wordt indien mogelijk behandeld als UStar. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *output* is niets. |
| ArgumentException | *output* is niet beschrijfbaar. |

### Opmerkingen

*output*moet beschrijfbaar zijn.

### Voorbeelden

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz"))
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

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)

---

## SaveLzipped(string, TarFormat?) {#savelzipped_1}

Slaat archief naar het bestand op pad met lzip-compressie.

```csharp
public void SaveLzipped(string path, TarFormat? format = default)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad van het aan te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| format | Nullable`1 | Definieert het formaat van de tar-koptekst. Null-waarde wordt indien mogelijk behandeld als UStar. |

### Voorbeelden

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.lz");
    }
}
```

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


