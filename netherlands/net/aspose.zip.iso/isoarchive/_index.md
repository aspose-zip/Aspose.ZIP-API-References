---
title: "Klasse IsoArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.Iso.IsoArchive class. Vertegenwoordigt een ISO-archief ISO 9660"
type: docs
weight: 570
url: /nl/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

Stelt een ISO-archief (ISO 9660) voor.

```csharp
public sealed class IsoArchive : IArchive
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | Initialiseert een nieuw exemplaar van de `IsoArchive` class en maakt een leeg ISO-archief aan voor het toevoegen van nieuwe bestanden en mappen. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | Initialiseert een nieuw exemplaar van de `IsoArchive` class en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | Initialiseert een nieuw exemplaar van de `IsoArchive` class en stelt een lijst met items samen die uit het archief kan worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | Haalt items van het type [`IsoEntry`](../isoentry/) op die het archief vormen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | Voegt een map toe aan het ISO‑beeld. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | Voegt een bestand toe aan het ISO‑beeld. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | Voegt een bestand toe aan het ISO‑beeld. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | Voegt een bestand toe aan het ISO‑beeld. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | Extraheert alle items naar de opgegeven map. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | Slaat het ISO‑beeld op in de opgegeven stream. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | Slaat het ISO‑beeld op op het opgegeven pad. |

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


