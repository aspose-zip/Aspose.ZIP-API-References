---
title: TarArchive.SaveZCompressed
second_title: Aspose.ZIP voor .NET API-referentie
description: TarArchive methode. Slaat archief op in de stream met Zcompressie.
type: docs
weight: 160
url: /nl/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

Slaat archief op in de stream met Z-compressie.

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

Slaat archief pad voor pad op met Z-compressie.

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
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
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* naamruimte [Aspose.Zip.Tar](../../tararchive/)
* montage [Aspose.Zip](../../../)


