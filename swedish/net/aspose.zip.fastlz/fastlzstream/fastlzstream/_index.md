---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP för .NET API-referens"
description: "FastLZStream-konstruktor. Initierar en ny instans av FastLZStream-klassen förberedd för komprimering."
type: docs
weight: 10
url: /sv/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Initierar en ny instans av [`FastLZStream`](../)-klassen förberedd för komprimering.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ström | Ström | Strömmen för att spara komprimerad data. |
| komprimeringsnivå | Int32 | Använd 1 för snabbare komprimering, använd 2 för ett bättre komprimeringsförhållande. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *stream* är null. |
| ArgumentException | *stream* stöder inte skrivning. |
| ArgumentOutOfRangeException | *compressionLevel* är mer än 2 eller mindre än 1. |

### Se även

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


