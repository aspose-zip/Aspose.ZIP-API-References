---
title: Class SevenZipArchiveEntryPlain
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain klass. SevenZippost som behöver komprimeras utan kryptering eller dekomprimeras utan dekryptering.
type: docs
weight: 690
url: /sv/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

SevenZip-post som behöver komprimeras utan kryptering eller dekomprimeras utan dekryptering.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
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
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | Extraherar posten till den tillhandahållna strömmen. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Öppnar posten för extraktion och tillhandahåller en ström med postinnehåll. |

## evenemang

| namn | Beskrivning |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Ökar när en del av råströmmen komprimeras. |

### Se även

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* namnutrymme [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* hopsättning [Aspose.Zip](../../)


