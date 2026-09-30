---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "CpioArchive method. Slaat het archief op in de stream met Z-compressie."
type: docs
weight: 130
url: /nl/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Slaat het archief op in de stream met Z-compressie.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Slaat het archief op naar het pad per pad met Z-compressie.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad van het te maken archief. Als de opgegeven bestandsnaam naar een bestaand bestand verwijst, wordt dit overschreven. |
| cpioFormat | CpioFormat | Definieert het cpio‑headerformaat. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| ArgumentNullException | *path* is `null`. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, (bijvoorbeeld, het bevindt zich op een niet-toegewezen station). |
| IOException | Er treedt een I/O-fout op. |
| PathTooLongException | Het opgegeven pad, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. |

## Voorbeelden

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Zie ook

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


