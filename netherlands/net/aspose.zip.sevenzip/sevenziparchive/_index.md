---
title: Class SevenZipArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.SevenZip.SevenZipArchive klas. Deze klasse vertegenwoordigt het 7zarchiefbestand. Gebruik het om 7zarchieven samen te stellen en uit te pakken.
type: docs
weight: 660
url: /nl/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Deze klasse vertegenwoordigt het 7z-archiefbestand. Gebruik het om 7z-archieven samen te stellen en uit te pakken.

```csharp
public class SevenZipArchive : IArchive
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Initialiseert een nieuw exemplaar van het`SevenZipArchive` klasse met optionele instellingen voor zijn ingangen. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Initialiseert een nieuw exemplaar van het`SevenZipArchive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Initialiseert een nieuw exemplaar van het`SevenZipArchive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Krijgt ingangen van[`SevenZipArchiveEntry`](../sevenziparchiveentry/) type waaruit het archief bestaat. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Compressie- en coderingsinstellingen gebruikt voor nieuw toegevoegde[`SevenZipArchiveEntry`](../sevenziparchiveentry/) artikelen. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de opgegeven map. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Maak een enkel item binnen het archief. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Pakt alle bestanden in het archief uit naar de opgegeven map. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Slaat 7z-archief op in de geleverde stream. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Slaat archief op in opgegeven bestemmingsbestand. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Slaat archief met meerdere volumes op in de opgegeven doelmap. |

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* naamruimte [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* montage [Aspose.Zip](../../)


