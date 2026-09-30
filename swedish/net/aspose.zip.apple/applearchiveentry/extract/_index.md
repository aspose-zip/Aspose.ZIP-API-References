---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AppleArchiveEntry metod. Extraherar posten till filsystemet med den angivna sökvägen"
type: docs
weight: 50
url: /sv/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Extraherar posten till filsystemet enligt den angivna sökvägen.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till destinationsfilen. Om filen redan finns, kommer den att skrivas över. |

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidDataException | Kontrollsumman eller digest som lagrats för posten matchar inte de extraherade data. |
| InvalidOperationException | Posten tillhör ett arkiv som förberetts för sammansättning, eller så kan postens data inte öppnas från en icke-sökbar arkivström. |
| NotSupportedException | Posten tillhör ett solid Apple Archive eller använder en ej stödd komprimeringsmetod. |
| ObjectDisposedException | Källströmmen har avlägsnats. |
| IOException | Ett I/O‑fel inträffar. |

### Se även

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraherar posten till den angivna strömmen.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Ström | Destinationsström. Måste vara skrivbar. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *destination* är `null`. |
| ArgumentException | *destination* stöder inte skrivning. |
| InvalidDataException | Kontrollsumman eller digest som lagrats för posten matchar inte de extraherade data. |
| InvalidOperationException | Posten tillhör ett arkiv som förberetts för sammansättning, eller så kan postens data inte öppnas från en icke-sökbar arkivström. |
| NotSupportedException | Posten tillhör ett solid Apple Archive eller använder en ej stödd komprimeringsmetod. |
| ObjectDisposedException | Källströmmen har avlägsnats. |
| IOException | Ett I/O‑fel inträffar. |

### Se även

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


