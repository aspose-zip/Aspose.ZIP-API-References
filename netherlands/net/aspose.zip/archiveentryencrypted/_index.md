---
title: Class ArchiveEntryEncrypted
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.ArchiveEntryEncrypted klas. Zipitem dat moet worden gecomprimeerd met codering of gedecomprimeerd met decodering.
type: docs
weight: 30
url: /nl/net/aspose.zip/archiveentryencrypted/
---
## ArchiveEntryEncrypted class

Zip-item dat moet worden gecomprimeerd met codering of gedecomprimeerd met decodering.

```csharp
public sealed class ArchiveEntryEncrypted : ArchiveEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | Krijgt commentaar van het item in archief. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | Krijgt grootte van gecomprimeerd bestand. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | Krijgt instellingen voor compressie of decompressie. |
| [EncryptionSettings](../../aspose.zip/archiveentryencrypted/encryptionsettings/) { get; } | Krijgt instellingen voor codering of decodering. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | Krijgt een waarde die aangeeft of de vermelding een directory vertegenwoordigt. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | Haalt of stelt de laatst gewijzigde datum en tijd in. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | Krijgt de naam van het item in het archief. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | Krijgt grootte van origineel bestand. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | Extraheert de ingang van de geleverde stream. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | Extraheert de invoer naar het bestandssysteem via het opgegeven pad. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | Opent het item voor extractie en biedt een stream met gedecomprimeerde inhoud van het item. |

## Evenementen

| Naam | Beschrijving |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | Verhoogt wanneer een deel van de onbewerkte stream wordt gecomprimeerd. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd. |

### Zie ook

* class [ArchiveEntry](../archiveentry/)
* naamruimte [Aspose.Zip](../../aspose.zip/)
* montage [Aspose.Zip](../../)


