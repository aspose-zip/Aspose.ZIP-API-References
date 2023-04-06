---
title: Class RarArchiveEntry
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Rar.RarArchiveEntry klas. Vertegenwoordigt enkel bestand binnen archief.
type: docs
weight: 320
url: /nl/net/aspose.zip.rar/rararchiveentry/
---
## RarArchiveEntry class

Vertegenwoordigt enkel bestand binnen archief.

```csharp
public abstract class RarArchiveEntry : IArchiveFileEntry
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | Krijgt grootte van gecomprimeerd bestand. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | Krijgt aanmaakdatum en -tijd. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | Krijgt een waarde die aangeeft of de vermelding een directory vertegenwoordigt. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | Krijgt datum en tijd van laatste toegang. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | Krijgt laatste gewijzigde datum en tijd. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | Krijgt de naam van het item in het archief. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | Krijgt grootte van origineel bestand. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract_1)(Stream, string) | Extraheert de ingang van de geleverde stream. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/#extract)(string, string) | Extraheert de invoer naar het bestandssysteem via het opgegeven pad. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | Opent het item voor extractie en biedt een stream met gedecomprimeerde inhoud van het item. |

## Evenementen

| Naam | Beschrijving |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | Verhoogt wanneer een deel van de onbewerkte stream wordt geëxtraheerd. |

### Opmerkingen

Werp een`RarArchiveEntry` bijvoorbeeld naar[`RarArchiveEntryEncrypted`](../rararchiveentryencrypted/) om te bepalen of de invoer is versleuteld of niet.

### Zie ook

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* naamruimte [Aspose.Zip.Rar](../../aspose.zip.rar/)
* montage [Aspose.Zip](../../)


