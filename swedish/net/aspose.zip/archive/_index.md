---
title: Class Archive
second_title: Aspose.ZIP för .NET API-referens
description: Aspose.Zip.Archive klass. Den här klassen representerar ziparkivfil. Använd den för att komponera extrahera eller uppdatera ziparkiv.
type: docs
weight: 10
url: /sv/net/aspose.zip/archive/
---
## Archive class

Den här klassen representerar zip-arkivfil. Använd den för att komponera, extrahera eller uppdatera zip-arkiv.

```csharp
public class Archive : IArchive
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | Initierar en ny instans av`Archive` klass med valfria inställningar för dess poster. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | Initierar en ny instans av`Archive` klass och komponerar poster lista kan extraheras från arkivet. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | Initierar en ny instans av`Archive` klass och komponerar poster lista kan extraheras från arkivet. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | Hämtar poster av[`ArchiveEntry`](../archiveentry/) typ som utgör arkivet. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | Komprimerings- och krypteringsinställningar som används för nyligen tillagda[`ArchiveEntry`](../archiveentry/) items. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | Lägger till alla filer och kataloger i arkivet rekursivt i den angivna katalogen. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | Skapa en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | Skapa en enskild post i arkivet. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | Tar bort den första förekomsten av en specifik post från postlistan. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | Tar bort posten från postlistan efter index. |
| [Dispose](../../aspose.zip/archive/dispose/)() | Utför programdefinierade uppgifter associerade med att frigöra, frigöra eller återställa ohanterade resurser. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | Extraherar alla filer i arkivet till den angivna katalogen. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | Sparar arkivet i den tillhandahållna strömmen. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | Sparar arkiv till destinationsfil som tillhandahålls. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | Sparar arkiv med flera volymer i den tillhandahållna destinationskatalogen. |

### Se även

* interface [IArchive](../iarchive/)
* namnutrymme [Aspose.Zip](../../aspose.zip/)
* hopsättning [Aspose.Zip](../../)


