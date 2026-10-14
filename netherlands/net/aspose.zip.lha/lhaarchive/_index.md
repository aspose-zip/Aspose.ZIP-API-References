---
title: "Klasse LhaArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "Aspose.Zip.Lha.LhaArchive klasse. Deze klasse vertegenwoordigt een LHA .lzh-archiefbestand"
type: docs
weight: 630
url: /nl/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Deze klasse vertegenwoordigt een LHA (.lzh)-archiefbestand.

```csharp
public class LhaArchive : IArchive
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Initialiseert een nieuw exemplaar van de `LhaArchive` klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Initialiseert een nieuw exemplaar van de `LhaArchive` klasse en stelt een lijst met items samen die uit het archief kunnen worden geëxtraheerd. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Haalt bestandsitems op van het type [`LhaArchiveEntry`](../lhaarchiveentry/) die het archief vormen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Extraheert alle bestanden en mappen in het archief naar de opgegeven map. |

## Opmerkingen

Alleen de volgende compressiemethoden worden ondersteund:

**Method**

**Explanation**

**lh0**

Niet gecomprimeerd

**lh4**

8 KiB glijdende woordenboek en statische Huffman

**lh5**

16 KiB glijdende woordenboek en statische Huffman

**lh6**

64 KiB glijdende woordenboek en statische Huffman

**lh7**

128 KiB glijdende woordenboek en statische Huffman

**lhx**

1 MiB glijdende woordenboek en statische Huffman

**lhd**

Map

### Zie ook

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


