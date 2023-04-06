---
title: Class SevenZipArchive
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.SevenZip.SevenZipArchive klass. Denna klass representerar 7z arkivfil. Använd den för att komponera och extrahera 7zarkiv.
type: docs
weight: 660
url: /sv/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

Denna klass representerar 7z arkivfil. Använd den för att komponera och extrahera 7z-arkiv.

```csharp
public class SevenZipArchive : IArchive
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | Initierar en ny instans av`SevenZipArchive` klass med valfria inställningar för dess poster. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | Initierar en ny instans av`SevenZipArchive` klass och komponerar poster lista kan extraheras från arkivet. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | Initierar en ny instans av`SevenZipArchive` klass och komponerar poster lista kan extraheras från arkivet. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | Hämtar poster av[`SevenZipArchiveEntry`](../sevenziparchiveentry/) typ som utgör arkivet. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | Komprimerings- och krypteringsinställningar som används för nyligen tillagda[`SevenZipArchiveEntry`](../sevenziparchiveentry/) items. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | Skapa en enskild post i arkivet. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | Extraherar alla filer i arkivet till den angivna katalogen. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | Sparar 7z-arkiv till den tillhandahållna strömmen. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | Sparar arkiv till destinationsfil som tillhandahålls. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | Sparar arkiv med flera volymer i den tillhandahållna destinationskatalogen. |

### Se även

* interface [IArchive](../../aspose.zip/iarchive/)
* namnutrymme [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* hopsättning [Aspose.Zip](../../)


