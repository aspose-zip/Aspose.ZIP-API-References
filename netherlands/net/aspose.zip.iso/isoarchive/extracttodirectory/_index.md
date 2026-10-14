---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "IsoArchive-methode. Extraheert alle items naar de opgegeven map"
type: docs
weight: 60
url: /nl/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Extraheert alle items naar de opgegeven map.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| destinationDirectory | String | De map waarin de items worden geëxtraheerd. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Wordt gegooid wanneer het archief zich in bewerkingsmodus bevindt. |
| ArgumentNullException | Wordt gegooid wanneer de *destinationDirectory* null is. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |

## Voorbeelden

Het volgende voorbeeld laat zien hoe alle items naar een map worden geëxtraheerd:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


