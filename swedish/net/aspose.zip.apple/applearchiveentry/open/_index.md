---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AppleArchiveEntry metod. Öppnar posten för extraktion och tillhandahåller en ström med postens innehåll"
type: docs
weight: 60
url: /sv/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Öppnar posten för extrahering och tillhandahåller en ström med postens innehåll.

```csharp
public Stream Open()
```

### Returvärde

En läsbar ström som innehåller de extraherade postdata.

### Undantag

| undantag | villkor |
| --- | --- |
| NotSupportedException | Posten tillhör ett solid Apple Archive eller använder en ej stödd komprimeringsmetod. |
| InvalidDataException | Kontrollsumman eller digest som lagrats för posten matchar inte de extraherade data. |
| InvalidOperationException | Posten tillhör ett arkiv som förberetts för sammansättning, eller så kan postens data inte öppnas från en icke-sökbar arkivström. |
| ObjectDisposedException | Källströmmen har avlägsnats. |
| IOException | Ett I/O‑fel inträffar. |

## Anmärkningar

Läs från den returnerade strömmen för att få det ursprungliga postinnehållet. Om arkivet innehåller kontrollsummafält verifieras kontrollsumman medan den returnerade strömmen läses.

### Se även

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


