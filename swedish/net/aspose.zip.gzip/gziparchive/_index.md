---
title: Class GzipArchive
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.Gzip.GzipArchive klass. Den här klassen representerar gziparkivfilen. Använd den för att komponera eller extrahera gziparkiv.
type: docs
weight: 210
url: /sv/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

Den här klassen representerar gzip-arkivfilen. Använd den för att komponera eller extrahera gzip-arkiv.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | Initierar en ny instans av`GzipArchive` klass förberedd för komprimering. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | Initierar en ny instans av`GzipArchive` klass förberedd för dekomprimering. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | Initierar en ny instans av`GzipArchive` class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | Namn på originalfil. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | Extraherar arkivet till den tillhandahållna strömmen. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | Öppnar arkivet för extrahering och tillhandahåller en ström med arkivinnehåll. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | Sparar arkivet i den tillhandahållna strömmen. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | Sparar arkiv till destinationsfil som tillhandahålls. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | Ställer in innehållet som ska komprimeras i arkivet. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | Ställer in innehållet som ska komprimeras i arkivet. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | Ställer in innehållet som ska komprimeras i arkivet. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | Ställer in innehållet som ska komprimeras i arkivet. |

### Anmärkningar

Gzip-komprimeringsalgoritmen är baserad på DEFLATE-algoritmen, som är en kombination av LZ77 och Huffman-kodning.

### Se även

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namnutrymme [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* hopsättning [Aspose.Zip](../../)


