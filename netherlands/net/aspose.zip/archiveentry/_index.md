---
title: Class ArchiveEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.ArchiveEntry klas. Vertegenwoordigt enkel bestand binnen archief.
type: docs
weight: 20
url: /nl/net/aspose.zip/archiveentry/
---
## ArchiveEntry class

Vertegenwoordigt enkel bestand binnen archief.

```csharp
public abstract class ArchiveEntry : IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Krijgt commentaar van het item in archief. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Krijgt grootte van gecomprimeerd bestand. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Krijgt instellingen voor compressie of decompressie. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Krijgt een waarde die aangeeft of de vermelding een directory vertegenwoordigt. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Haalt of stelt de laatst gewijzigde datum en tijd in. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Krijgt de naam van het item in het archief. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Krijgt grootte van origineel bestand. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/#extract_1)(Stream, string) | Extraheert de ingang van de geleverde stream. |
| [Extract](../../aspose.zip/archiveentry/extract/#extract)(string, string) | Extraheert de invoer naar het bestandssysteem via het opgegeven pad. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Opent het item voor extractie en biedt een stream met gedecomprimeerde inhoud van het item. |

## Evenementen

| Naam | Beschrijving |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd. |

### Opmerkingen

Werp een`ArchiveEntry` bijvoorbeeld naar[`ArchiveEntryEncrypted`](../archiveentryencrypted/) om te bepalen of de invoer is versleuteld of niet.

### Zie ook

* interface [IArchiveFileEntry](../iarchivefileentry/)
* naamruimte [Aspose.Zip](../../aspose.zip/)
* montage [Aspose.Zip](../../)


