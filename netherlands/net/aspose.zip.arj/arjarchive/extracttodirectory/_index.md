---
title: "ArjArchive.ExtractToDirectory"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ArjArchive-methode. Extraheert alle items naar de opgegeven map."
type: docs
weight: 60
url: /nl/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Wordt gegooid wanneer de *destinationDirectory* null is. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| InvalidDataException | Controlesom komt niet overeen voor headers of data. - of - Archief is corrupt. |
| NotImplementedException | Item gecomprimeerd met methode 4. |

## Voorbeelden

Het volgende voorbeeld laat zien hoe alle items naar een map worden geëxtraheerd:

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Zie ook

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


