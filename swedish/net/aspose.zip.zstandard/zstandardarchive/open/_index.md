---
title: "ZstandardArchive.Open"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZstandardArchive-metod. Öppnar arkivet för extraktion och tillhandahåller en ström med arkivinnehåll"
type: docs
weight: 50
url: /sv/net/aspose.zip.zstandard/zstandardarchive/open/
---
## ZstandardArchive.Open method

Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehållet.

```csharp
public Stream Open()
```

### Returvärde

Strömmen som representerar arkivets innehåll.

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

Läs från strömmen för att få originalinnehållet i en fil. Se avsnittet exempel.

## Exempel

Extraherar arkivet och kopierar det extraherade innehållet till filströmmen.

```csharp
using (var archive = new ZstandardArchive("archive.zst"))
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

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


