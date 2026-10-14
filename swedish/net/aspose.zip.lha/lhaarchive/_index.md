---
title: "Klass LhaArchive"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Aspose.Zip.Lha.LhaArchive-klass. Denna klass representerar en LHA .lzh-arkivfil"
type: docs
weight: 630
url: /sv/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Denna klass representerar en LHA (.lzh)-arkivfil.

```csharp
public class LhaArchive : IArchive
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Initierar en ny instans av klassen `LhaArchive` och sammansätter en postlista som kan extraheras från arkivet. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Initierar en ny instans av klassen `LhaArchive` och sammansätter en postlista som kan extraheras från arkivet. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Hämtar filposter av typen [`LhaArchiveEntry`](../lhaarchiveentry/) som utgör arkivet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Extraherar alla filer och kataloger i arkivet till den angivna katalogen. |

## Anmärkningar

Endast följande komprimeringsmetoder stöds:

**Method**

**Explanation**

**lh0**

Okomprimerad

**lh4**

8 KiB glidande ordbok och statisk Huffman

**lh5**

16 KiB glidande ordbok och statisk Huffman

**lh6**

64 KiB glidande ordbok och statisk Huffman

**lh7**

128 KiB glidande ordbok och statisk Huffman

**lhx**

1 Mib glidande ordbok och statisk Huffman

**lhd**

Katalog

### Se även

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


