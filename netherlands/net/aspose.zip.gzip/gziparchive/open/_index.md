---
title: GzipArchive.Open
second_title: Aspose.ZIP voor .NET API-referentie
description: GzipArchive methode. Opent het archief voor extractie en levert een stream met archiefinhoud.
type: docs
weight: 50
url: /nl/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Opent het archief voor extractie en levert een stream met archiefinhoud.

```csharp
public Stream Open()
```

### Winstwaarde

De stream die de inhoud van het archief vertegenwoordigt.

### Opmerkingen

Lees uit de stream om de originele inhoud van het bestand te krijgen. Zie voorbeelden sectie.

### Voorbeelden

Pakt het archief uit en kopieert de geëxtraheerde inhoud naar de bestandsstroom.

U mag de Stream.CopyTo-methode gebruiken voor .NET 4.0 en hoger:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
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

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)


