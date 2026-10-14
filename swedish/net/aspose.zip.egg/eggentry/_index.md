---
title: "Klass EggEntry"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Egg.EggEntry klass. Representerar en filpost i ett EGG-arkiv med all dess metadata"
type: docs
weight: 470
url: /sv/net/aspose.zip.egg/eggentry/
---
## EggEntry class

Representerar en filpost i ett EGG-arkiv med all dess metadata.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | Hämtar den komprimerade storleken på posten. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | Hämtar ett värde som indikerar om denna post representerar en katalog. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | Hämtar eller anger senast ändrat datum och -tid. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | Hämtar namnet på posten i arkivet. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | Hämtar den okomprimerade storleken på posten. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | Extraherar posten till den angivna strömmen. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | Extraherar posten till filsystemet enligt den angivna sökvägen. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | Öppnar posten för extrahering och tillhandahåller en ström med dekomprimerat postinnehåll. |

### Se även

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


