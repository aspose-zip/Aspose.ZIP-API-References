---
title: "TarArchive.SaveLZ4Compressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "TarArchive-methode. Slaat het archief op in de stream met LZ4-compressie"
type: docs
weight: 170
url: /nl/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

Slaat het archief op in de stream met LZ4-compressie.

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uitvoer | Stream | Doelstream. |
| formaat | Nullable`1 | Definieert het tar-headerformaat. Een null-waarde wordt, indien mogelijk, behandeld als USTar. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is niet beschrijfbaar. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt |
| IOException | Er treedt een I/O-fout op. |

## Opmerkingen

*output* must be writable.

## Voorbeelden

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

Slaat het archief op in het bestand via pad met LZ4-compressie.

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| formaat | Nullable`1 | Definieert het tar-headerformaat. Een null-waarde wordt, indien mogelijk, behandeld als USTar. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| UnauthorizedAccessException | De aanroeper heeft niet de vereiste toestemming. -of- *path* gaf een alleen-lezen bestand of map op. |
| ArgumentException | *path* is een tekenreeks met lengte nul, bevat alleen witruimte, of bevat één of meer ongeldige tekens zoals gedefinieerd door InvalidPathChars. |
| ArgumentNullException | *path* is null. |
| PathTooLongException | Het opgegeven *path*, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. Bijvoorbeeld, op Windows-platformen moeten paden korter zijn dan 248 tekens, en bestandsnamen korter dan 260 tekens. |
| DirectoryNotFoundException | Het opgegeven *path* is ongeldig (bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt). |
| NotSupportedException | *path* heeft een ongeldig formaat. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt |
| IOException | Er treedt een I/O-fout op. |

## Voorbeelden

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


