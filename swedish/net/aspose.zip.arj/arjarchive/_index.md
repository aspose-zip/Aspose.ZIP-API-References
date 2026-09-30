---
title: "Klass ArjArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Arj.ArjArchive-klass. Denna klass representerar en ARJ-arkivfil"
type: docs
weight: 250
url: /sv/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Denna klass representerar en ARJ-arkivfil.

```csharp
public class ArjArchive : IArchive
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Initierar en ny instans av `ArjArchive`-klassen och skapar en postlista som kan extraheras från arkivet. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Initierar en ny instans av `ArjArchive`-klassen och skapar en postlista som kan extraheras från arkivet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Hämtar kommentaren. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Hämtar poster av typen [`ArjEntryPlain`](../arjentryplain/) som utgör ARJ-arkivet. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Hämtar det ursprungliga namnet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Extraherar alla poster till den angivna katalogen. |

## Anmärkningar

Endast följande komprimeringsmetoder stöds:

**Method**

**Explanation**

**0**

Okomprimerad

**1**

Kombination av LZ77 och adaptiv Huffman-kodning. Bästa komprimeringsförhållande.

**2**

Kombination av LZ77 och adaptiv Huffman-kodning.

**3**

Kombination av LZ77 och adaptiv Huffman-kodning. Bästa hastigheten.

### Se även

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


