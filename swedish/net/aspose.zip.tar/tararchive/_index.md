---
title: TarArchive
second_title: Aspose.ZIP för .NET API-referens
description: Denna klass representerar tar arkivfil. Använd den för att komponera extrahera eller uppdatera tararkiv.
type: docs
weight: 600
url: /sv/net/aspose.zip.tar/tararchive/
---
## TarArchive class

Denna klass representerar tar arkivfil. Använd den för att komponera, extrahera eller uppdatera tar-arkiv.

```csharp
public class TarArchive : IDisposable
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [TarArchive](tararchive#constructor)() | Initierar en ny instans av[`TarArchive`](../tararchive) class. |
| [TarArchive](tararchive#constructor_1)(Stream) | Initierar en ny instans av[`Archive`](../../aspose.zip/archive) klass och komponerar poster lista kan extraheras från arkivet. |
| [TarArchive](tararchive#constructor_2)(string) | Initierar en ny instans av[`TarArchive`](../tararchive) klass och komponerar poster lista kan extraheras från arkivet. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries) { get; } | Hämtar poster av[`TarEntry`](../tarentry) typ som utgör arkivet. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip)(Stream) | Extraherar medföljande gzip-arkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip#fromgzip_1)(string) | Extraherar medföljande gzip-arkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip)(Stream) | Extraherar medföljande lzip-arkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip#fromlzip_1)(string) | Extraherar medföljande lzip-arkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz)(Stream) | Extraherar medföljande xz-formatarkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz#fromxz_1)(string) | Extraherar medföljande xz-formatarkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz)(Stream) | Extraherar medföljande Z-formatarkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz#fromz_1)(string) | Extraherar medföljande Z-formatarkiv och komponerar[`TarArchive`](../tararchive) från extraherade data. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries)(DirectoryInfo, bool) | Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries#createentries_1)(string, bool) | Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry)(string, FileInfo, bool) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_1)(string, Stream, FileSystemInfo) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry#createentry_2)(string, string, bool) | Skapa en enskild post i arkivet. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry_1)(int) | Tar bort posten från postlistan efter index. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry#deleteentry)(TarEntry) | Tar bort den första förekomsten av en specifik post från postlistan. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory)(string) | Extraherar alla filer i arkivet till den angivna katalogen. |
| [Save](../../aspose.zip.tar/tararchive/save#save)(Stream, TarFormat?) | Sparar arkivet i den tillhandahållna strömmen. |
| [Save](../../aspose.zip.tar/tararchive/save#save_1)(string, TarFormat?) | Sparar arkiv till destinationsfil som tillhandahålls. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped)(Stream, TarFormat?) | Sparar arkiv i strömmen med gzip-komprimering. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped#savegzipped_1)(string, TarFormat?) | Sparar arkiv till filen efter sökväg med gzip-komprimering. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped)(Stream, TarFormat?) | Sparar arkiv i strömmen med lzip-komprimering. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped#savelzipped_1)(string, TarFormat?) | Sparar arkiv till filen efter sökväg med lzip-komprimering. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | Sparar arkiv till strömmen med xz-komprimering. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | Sparar arkiv till sökvägen för sökväg med xz-komprimering. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed)(Stream, TarFormat?) | Sparar arkiv i strömmen med Z-komprimering. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed#savezcompressed_1)(string, TarFormat?) | Sparar arkiv till sökvägen för sökväg med Z-komprimering. |

### Se även

* namnutrymme [Aspose.Zip.Tar](../../aspose.zip.tar)
* hopsättning [Aspose.Zip](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Zip.dll -->
