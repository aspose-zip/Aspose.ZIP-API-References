---
title: "TarArchive.SaveZstandard"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "TarArchive-methode. Slaat het archief op in de stream met Zstandard-compressie"
type: docs
weight: 220
url: /nl/net/aspose.zip.tar/tararchive/savezstandard/
---
## SaveZstandard(Stream, TarFormat?) {#savezstandard}

Slaat het archief op in de stream met Zstandard-compressie.

```csharp
public void SaveZstandard(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, TarFormat?) {#savezstandard_1}

Slaat het archief op in het bestand op het opgegeven pad met Zstandard-compressie.

```csharp
public void SaveZstandard(string path, TarFormat? format = default)
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

## Voorbeelden

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.tar.zst");
    }
}
```

### Zie ook

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


