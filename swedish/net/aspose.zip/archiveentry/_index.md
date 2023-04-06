---
title: Class ArchiveEntry
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.ArchiveEntry klass. Representerar en fil i arkivet.
type: docs
weight: 20
url: /sv/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Representerar en fil i arkivet.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Får kommentar av posten i arkivet. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Hämtar storleken på den komprimerade filen. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Hämtar inställningar för komprimering eller dekompression. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Får ett värde som indikerar om posten representerar katalog. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Hämtar eller ställer in datum och tid för senaste ändring. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Hämtar namnet på posten i arkivet. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Hämtar storleken på originalfilen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Extraherar posten till den tillhandahållna strömmen. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |

## evenemang

| namn | Beskrivning |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Ökar när en del av råströmmen komprimeras. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Ökar när en del av råström extraheras. |

### Anmärkningar

Kasta en`ArchiveEntry` instans till[`ArchiveEntryEncrypted`](../archiveentryencrypted/) för att avgöra om posten är krypterad eller inte.

### Se även

* interface [IArchiveFileEntry](../iarchivefileentry/)
* namnutrymme [Aspose.Zip](../../aspose.zip/)
* hopsättning [Aspose.Zip](../../)


