---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Lz4Archive metod. Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehållet"
type: docs
weight: 50
url: /sv/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehållet.

```csharp
public Stream Open()
```

### Returvärde

Strömmen som representerar arkivets innehåll.

### Undantag

| undantag | villkor |
| --- | --- |
| EndOfStreamException | Källströmmen är för kort. |
| InvalidDataException | Felaktiga byte hittades vid initiering av avkodning. |
| InvalidOperationException | Arkivet är förberett för sammansättning. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| IOException | Ett I/O‑fel inträffar. |

## Anmärkningar

Läs från strömmen för att få originalinnehållet i en fil. Se avsnittet exempel.

## Exempel

Extraherar arkivet och kopierar det extraherade innehållet till filströmmen.

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

Du kan använda Stream.CopyTo-metoden för .NET 4.0 och högre:

```csharp
unpacked.CopyTo(extracted);
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


