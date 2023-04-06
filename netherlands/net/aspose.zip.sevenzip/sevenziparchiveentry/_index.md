---
title: Class SevenZipArchiveEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry klas. Vertegenwoordigt enkel bestand binnen 7zarchief.
type: docs
weight: 670
url: /nl/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

Vertegenwoordigt enkel bestand binnen 7z-archief.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | Krijgt grootte van gecomprimeerd bestand. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | Krijgt instellingen voor compressie of decompressie. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | Krijgt een waarde die aangeeft of de vermelding een directory vertegenwoordigt. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | Krijgt laatste gewijzigde datum en tijd. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | Krijgt de naam van het item in het archief. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | Krijgt grootte van origineel bestand. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | Extraheert de ingang van de geleverde stream. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | Extraheert de invoer naar het bestandssysteem via het opgegeven pad. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | Opent het item voor extractie en biedt een stream met inhoud van het item. |

## Evenementen

| Naam | Beschrijving |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd. |

### Opmerkingen

Werp een`SevenZipArchiveEntry` bijvoorbeeld naar[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) om te bepalen of de invoer is versleuteld of niet.

### Zie ook

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* naamruimte [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* montage [Aspose.Zip](../../)


