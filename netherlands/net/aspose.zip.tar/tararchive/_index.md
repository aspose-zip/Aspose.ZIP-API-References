---
title: Class TarArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: Aspose.Zip.Tar.TarArchive klas. Deze klasse vertegenwoordigt een tararchiefbestand. Gebruik het om tararchieven samen te stellen uit te pakken of bij te werken.
type: docs
weight: 730
url: /nl/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Deze klasse vertegenwoordigt een tar-archiefbestand. Gebruik het om tar-archieven samen te stellen, uit te pakken of bij te werken.

```csharp
public class TarArchive : IArchive
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | Initialiseert een nieuw exemplaar van het`TarArchive` klasse. |
| [TarArchive](tararchive/#constructor_1)(Stream) | Initialiseert een nieuw exemplaar van het[`Archive`](../../aspose.zip/archive/) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |
| [TarArchive](tararchive/#constructor_2)(string) | Initialiseert een nieuw exemplaar van het`TarArchive` klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | Krijgt ingangen van[`TarEntry`](../tarentry/) type waaruit het archief bestaat. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | Extraheert geleverd gzip-archief en stelt samen`TarArchive` uit geëxtraheerde gegevens. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | Extraheert geleverd gzip-archief en stelt samen`TarArchive` uit geëxtraheerde gegevens. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | Extraheert geleverd lzip-archief en stelt samen`TarArchive` uit geëxtraheerde gegevens. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | Extraheert geleverd lzip-archief en stelt samen`TarArchive` uit geëxtraheerde gegevens. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | Extracten geleverd xz formaat archief en componeert`TarArchive` uit geëxtraheerde gegevens. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | Extracten geleverd xz formaat archief en componeert`TarArchive` uit geëxtraheerde gegevens. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | Extraheert geleverd archief in Z-formaat en stelt samen`TarArchive` uit geëxtraheerde gegevens. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | Extraheert geleverd archief in Z-formaat en stelt samen`TarArchive` uit geëxtraheerde gegevens. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | Voegt recursief alle bestanden en mappen toe aan het archief in de gegeven map. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | Maak een enkel item binnen het archief. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | Maak een enkel item binnen het archief. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | Verwijdert het item uit de lijst met items op index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | Verwijdert het eerste exemplaar van een specifiek item uit de lijst met items. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijmaken, vrijgeven of resetten van onbeheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | Pakt alle bestanden in het archief uit naar de opgegeven map. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | Slaat archief op in de geleverde stream. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | Slaat archief op in opgegeven bestemmingsbestand. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | Slaat archief op in de stream met gzip-compressie. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | Slaat archief naar het bestand op pad met gzip-compressie. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | Slaat archief op in de stream met lzip-compressie. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | Slaat archief naar het bestand op pad met lzip-compressie. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Slaat archief op in de stream met xz-compressie. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Slaat archief pad voor pad op met xz-compressie. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Slaat archief op in de stream met Z-compressie. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Slaat archief pad voor pad op met Z-compressie. |

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* naamruimte [Aspose.Zip.Tar](../../aspose.zip.tar/)
* montage [Aspose.Zip](../../)


