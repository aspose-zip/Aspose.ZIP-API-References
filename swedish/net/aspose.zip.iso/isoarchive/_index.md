---
title: "Klass IsoArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Iso.IsoArchive-klass. Representerar ett ISO-arkiv ISO 9660"
type: docs
weight: 570
url: /sv/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Representerar ett ISO-arkiv (ISO 9660).

```csharp
public sealed class IsoArchive : IArchive
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Initierar en ny instans av `IsoArchive`-klassen och skapar ett tomt ISO-arkiv för att lägga till nya filer och kataloger. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Initierar en ny instans av `IsoArchive`-klassen och sammanställer en postlista som kan extraheras från arkivet. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Initierar en ny instans av `IsoArchive`-klassen och sammanställer en postlista som kan extraheras från arkivet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Hämtar poster av typen [`IsoEntry`](../isoentry/) som utgör arkivet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Lägger till en katalog i ISO-avbilden. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Lägger till en fil i ISO-avbilden. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Lägger till en fil i ISO-avbilden. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Lägger till en fil i ISO-avbilden. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Utför applikationsdefinierade uppgifter som är relaterade till att frigöra, släppa eller återställa ohanterade resurser. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Extraherar alla poster till den angivna katalogen. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Sparar ISO-avbilden till den angivna strömmen. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Sparar ISO-avbilden till den angivna sökvägen. |

### Se även

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


