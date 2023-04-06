---
title: Class ArchiveEntryPlain
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.ArchiveEntryPlain klass. Zippost som måste komprimeras utan kryptering eller dekomprimeras utan dekryptering.
type: docs
weight: 40
url: /sv/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

Zip-post som måste komprimeras utan kryptering eller dekomprimeras utan dekryptering.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
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
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Extraherar posten till den tillhandahållna strömmen. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |

## evenemang

| namn | Beskrivning |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Ökar när en del av råströmmen komprimeras. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Ökar när en del av råström extraheras. |

### Se även

* class [ArchiveEntry](../archiveentry/)
* namnutrymme [Aspose.Zip](../../aspose.zip/)
* hopsättning [Aspose.Zip](../../)


