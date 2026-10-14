---
title: "Klass AppleArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Apple.AppleArchive klass. Denna klass representerar en Apple Archive .aar-fil. Använd den för att komponera Apple Archive-filer."
type: docs
weight: 60
url: /sv/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Denna klass representerar en Apple Archive (.aar)-fil. Använd den för att skapa Apple Archive-filer.

```csharp
public class AppleArchive : IArchive
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Initierar en ny instans av `AppleArchive`-klassen med inställningar som används för sammansatta poster. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Initierar en ny instans av `AppleArchive`-klassen och komponera en postlista som kan extraheras från arkivet. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Initierar en ny instans av `AppleArchive`-klassen och komponera en postlista som kan extraheras från arkivet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Hämtar poster som utgör arkivet. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Hämtar ett värde som indikerar om arkivet använder solid kompression. I solid läge komprimeras all postdata som en enda ström och individuell postextraktion är inte tillgänglig. Använd [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) istället. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Hämtar inställningar som används för nykomponerade poster. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Lägger till alla filer och kataloger rekursivt i den angivna katalogen i arkivet. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Skapar en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Skapar en enskild post i arkivet. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Skapar en enskild post i arkivet. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Extraherar alla filer i arkivet till den angivna katalogen. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Sparar arkivet till den angivna strömmen. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Sparar arkivet till en angiven destinationsfil. |

## Anmärkningar

Apple och Apple Archive är varumärken som tillhör Apple Inc.

### Se även

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


