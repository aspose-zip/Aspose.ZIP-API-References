---
title: "Klasse ArjArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.Arj.ArjArchive klasse. Deze klasse vertegenwoordigt een ARJ-archiefbestand."
type: docs
weight: 250
url: /nl/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Deze klasse vertegenwoordigt een ARJ-archiefbestand.

```csharp
public class ArjArchive : IArchive
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Initialiseert een nieuw exemplaar van de `ArjArchive` klasse en stelt een lijst met items samen die uit het archief kunnen worden gehaald. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Initialiseert een nieuw exemplaar van de `ArjArchive` klasse en stelt een lijst met items samen die uit het archief kunnen worden gehaald. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Haalt het commentaar op. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Haalt items op van het type [`ArjEntryPlain`](../arjentryplain/) die het ARJ-archief vormen. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Haalt de oorspronkelijke naam op. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Voert door de toepassing gedefinieerde taken uit die verband houden met het vrijgeven, loslaten of resetten van niet-beheerde bronnen. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Extraheert alle items naar de opgegeven map. |

## Opmerkingen

Alleen de volgende compressiemethoden worden ondersteund:

**Method**

**Explanation**

**0**

Niet gecomprimeerd

**1**

Combinatie van LZ77 en adaptieve Huffman-codering. Beste compressieverhouding.

**2**

Combinatie van LZ77 en adaptieve Huffman-codering.

**3**

Combinatie van LZ77 en adaptieve Huffman-codering. Beste snelheid.

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


