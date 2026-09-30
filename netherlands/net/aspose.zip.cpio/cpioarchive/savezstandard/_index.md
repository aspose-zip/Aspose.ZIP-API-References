---
title: "CpioArchive.SaveZstandard"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "CpioArchive method. Slaat het archief op in de stream met Zstandard-compressie."
type: docs
weight: 140
url: /nl/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Slaat het archief op in de stream met Zstandard-compressie.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uitvoer | Stream | Doelstream. |
| cpioFormat | CpioFormat | Definieert het cpio‑headerformaat. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *output* is null. |
| ArgumentException | *output* is niet beschrijfbaar. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Opmerkingen

*output* must be writable.

## Voorbeelden

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
        }
    }
}
```

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Slaat het archief op in het bestand op het opgegeven pad met Zstandard-compressie.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| cpioFormat | CpioFormat | Definieert het cpio‑headerformaat. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentException | *path* is een tekenreeks met lengte nul, bevat alleen witruimte, of bevat één of meer ongeldige tekens zoals gedefinieerd door InvalidPathChars. |
| ArgumentNullException | *path* is `null`. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, (bijvoorbeeld, het bevindt zich op een niet-toegewezen station). |
| IOException | Er treedt een I/O-fout op. |
| PathTooLongException | Het opgegeven pad, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. |
| UnauthorizedAccessException | De aanroeper heeft niet de vereiste toestemming. -of- *path* gaf een alleen-lezen bestand of map op. |

## Voorbeelden

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


