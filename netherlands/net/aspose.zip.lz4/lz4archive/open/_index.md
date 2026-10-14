---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Lz4Archive methode. Opent het archief voor extractie en levert een stroom met de archiefinhoud."
type: docs
weight: 50
url: /nl/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Opent het archief voor extractie en levert een stream met de archiefinhoud.

```csharp
public Stream Open()
```

### Retourwaarde

De stream die de inhoud van het archief vertegenwoordigt.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| EndOfStreamException | Bronstroom is te kort. |
| InvalidDataException | Verkeerde bytes gevonden tijdens het initialiseren van decodering. |
| InvalidOperationException | Het archief is voorbereid op samenstelling. |
| ObjectDisposedException | Archief is verwijderd en kan niet worden gebruikt. |
| IOException | Er treedt een I/O-fout op. |

## Opmerkingen

Lees van de stream om de oorspronkelijke inhoud van een bestand te verkrijgen. Zie de sectie voorbeelden.

## Voorbeelden

Extraheert het archief en kopieert de geëxtraheerde inhoud naar een bestandsstroom.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

U kunt de Stream.CopyTo-methode gebruiken voor .NET 4.0 en hoger:

```csharp
unpacked.CopyTo(extracted);
```

### Zie ook

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


