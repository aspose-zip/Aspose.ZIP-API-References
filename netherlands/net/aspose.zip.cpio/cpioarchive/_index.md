---
title: Class CpioArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Cpio.CpioArchive klas. Deze klasse vertegenwoordigt cpioarchiefbestand.
type: docs
weight: 160
url: /nl/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

Deze klasse vertegenwoordigt cpio-archiefbestand.

```csharp
public class CpioArchive : IArchive
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | Initialiseert een nieuw exemplaar van het`CpioArchive` klasse. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | Initialiseert een nieuw exemplaar van het`CpioArchive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | Initialiseert een nieuw exemplaar van het`CpioArchive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | Krijgt ingangen van[`CpioEntry`](../cpioentry/) type waaruit het archief bestaat. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | Maak een enkel item binnen het archief. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | Verwijdert het item uit de lijst met items op index. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | Pakt alle bestanden in het archief uit naar de opgegeven map. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | Slaat archief op in de geleverde stream. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | Slaat archief op in opgegeven bestemmingsbestand. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | Slaat archief op in de stream met gzip-compressie. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | Slaat archief naar het bestand op pad met gzip-compressie. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | Slaat archief op in de stream met xz-compressie. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | Slaat archief pad voor pad op met xz-compressie. |

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* naamruimte [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* montage [Aspose.Zip](../../)


