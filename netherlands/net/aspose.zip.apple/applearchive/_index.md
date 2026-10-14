---
title: "Klasse AppleArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.Apple.AppleArchive class. Deze klasse vertegenwoordigt een Apple Archive .aar‑bestand. Gebruik deze om Apple Archive‑bestanden samen te stellen."
type: docs
weight: 60
url: /nl/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

Deze klasse vertegenwoordigt een Apple Archive (.aar)-bestand. Gebruik het om Apple Archive-bestanden samen te stellen.

```csharp
public class AppleArchive : IArchive
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | Initialiseert een nieuw exemplaar van de `AppleArchive` class met instellingen die worden gebruikt voor samengestelde items. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | Initialiseert een nieuw exemplaar van de `AppleArchive` class en stelt een itemslijst samen die uit het archief kan worden geëxtraheerd. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | Initialiseert een nieuw exemplaar van de `AppleArchive` class en stelt een itemslijst samen die uit het archief kan worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | Haalt de items op die het archief vormen. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | Haalt een waarde op die aangeeft of het archief solide compressie gebruikt. In solide modus wordt alle itemdata gecomprimeerd als één enkele stroom en is individuele itemextractie niet beschikbaar. Gebruik [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/) in plaats daarvan. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | Haalt de instellingen op die worden gebruikt voor nieuw samengestelde items. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | Voegt alle bestanden en mappen recursief uit de opgegeven map toe aan het archief. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | Maakt een enkel item binnen het archief aan. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | Maakt een enkel item binnen het archief aan. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | Maakt een enkel item binnen het archief aan. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | Extraheert alle bestanden in het archief naar de opgegeven map. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | Slaat het archief op in de opgegeven stream. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | Slaat het archief op in een opgegeven bestemmingsbestand. |

## Opmerkingen

Apple en Apple Archive zijn handelsmerken van Apple Inc.

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


