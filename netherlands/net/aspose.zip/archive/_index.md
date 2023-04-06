---
title: Class Archive
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Archive klas. Deze klasse vertegenwoordigt een ziparchiefbestand. Gebruik het om ziparchieven samen te stellen uit te pakken of bij te werken.
type: docs
weight: 10
url: /nl/net/aspose.zip/archive/
---
## Archive class

Deze klasse vertegenwoordigt een zip-archiefbestand. Gebruik het om zip-archieven samen te stellen, uit te pakken of bij te werken.

```csharp
public class Archive : IArchive
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Initialiseert een nieuw exemplaar van het`Archive` klasse met optionele instellingen voor zijn ingangen. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Initialiseert een nieuw exemplaar van het`Archive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Initialiseert een nieuw exemplaar van het`Archive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Krijgt ingangen van[`ArchiveEntry`](../archiveentry/) type waaruit het archief bestaat. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Compressie- en coderingsinstellingen gebruikt voor nieuw toegevoegde[`ArchiveEntry`](../archiveentry/) artikelen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Maak een enkel item binnen het archief. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Verwijdert het item uit de lijst met items op index. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Pakt alle bestanden in het archief uit naar de opgegeven map. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Slaat archief op in de geleverde stream. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Slaat archief op in opgegeven bestemmingsbestand. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Slaat archief met meerdere volumes op in de opgegeven doelmap. |

### Zie ook

* interface [IArchive](../iarchive/)
* naamruimte [Aspose.Zip](../../aspose.zip/)
* montage [Aspose.Zip](../../)


