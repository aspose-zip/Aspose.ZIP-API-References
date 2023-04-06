---
title: Class RarArchiveEntry
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.Rar.RarArchiveEntry klass. Representerar en fil i arkivet.
type: docs
weight: 320
url: /sv/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Representerar en fil i arkivet.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Hämtar storleken på den komprimerade filen. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Hämtar datum och tid för skapande. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Får ett värde som indikerar om posten representerar katalog. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Får senaste åtkomstdatum och tid. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Hämtar senast ändrad datum och tid. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Hämtar namnet på posten i arkivet. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Hämtar storleken på originalfilen. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Extraherar posten till den tillhandahållna strömmen. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Extraherar posten till filsystemet med den angivna sökvägen. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Öppnar posten för extraktion och tillhandahåller en ström med dekomprimerat postinnehåll. |

## evenemang

| namn | Beskrivning |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Ökar när en del av råström extraheras. |

### Anmärkningar

Kasta en`RarArchiveEntry` instans till[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) för att avgöra om posten är krypterad eller inte.

### Se även

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namnutrymme [Aspose.Zip.Rar](../../aspose.zip.rar/)
* hopsättning [Aspose.Zip](../../)


