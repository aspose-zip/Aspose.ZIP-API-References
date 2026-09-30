---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP för .NET API-referens"
description: "FastLZStream metod. Läser en sekvens av byte från strömmen och avancerar positionen i strömmen med antalet lästa byte. Stöds inte"
type: docs
weight: 90
url: /sv/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Läser en sekvens av byte från strömmen och avancerar positionen i strömmen med antalet lästa byte. Stöds inte.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| buffert | Byte[] | En array av byte. När denna metod returnerar innehåller bufferten den specificerade bytearrayen med värdena mellan offset och (offset + count - 1) ersatta av de byte som lästs från den aktuella källan. |
| förskjutning | Int32 | Det nollbaserade byteoffsetet i buffert där lagringen av data läst från den aktuella strömmen ska börja. |
| count | Int32 | Det maximala antalet byte som ska läsas från den aktuella strömmen. |

### Returvärde

Det totala antalet byte som lästs in i bufferten. Detta kan vara mindre än det begärda antalet byte om så många byte för närvarande inte är tillgängliga, eller noll (0) om slutet av strömmen har nåtts.

### Undantag

| undantag | villkor |
| --- | --- |
| NotSupportedException | Operationen stöds inte. |

### Se även

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


