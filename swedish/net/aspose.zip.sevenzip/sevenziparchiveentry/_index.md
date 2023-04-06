---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry klass. Representerar en fil i 7zarkiv.
type: docs
weight: 670
url: /sv/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Representerar en fil i 7z-arkiv.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Hämtar storleken på den komprimerade filen. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Hämtar inställningar för komprimering eller dekompression. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Får ett värde som indikerar om posten representerar katalog. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Hämtar senast ändrad datum och tid. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Hämtar namnet på posten i arkivet. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Hämtar storleken på originalfilen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Extraherar posten till den tillhandahållna strömmen. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Öppnar posten för extraktion och tillhandahåller en ström med postinnehåll. |

## evenemang

| namn | Beskrivning |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Ökar när en del av råströmmen komprimeras. |

### Anmärkningar

Kasta en`SevenZipArchiveEntry` instans till[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) för att avgöra om posten är krypterad eller inte.

### Se även

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namnutrymme [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* hopsättning [Aspose.Zip](../../)


