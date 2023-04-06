---
title: Class ArchiveEntryEncrypted
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.ArchiveEntryEncrypted klass. Zippost som måste komprimeras med kryptering eller dekomprimeras med dekryptering.
type: docs
weight: 30
url: /sv/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Zip-post som måste komprimeras med kryptering eller dekomprimeras med dekryptering.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Får kommentar av posten i arkivet. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Hämtar storleken på den komprimerade filen. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Hämtar inställningar för komprimering eller dekompression. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Hämtar inställningar för kryptering eller dekryptering. |
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


