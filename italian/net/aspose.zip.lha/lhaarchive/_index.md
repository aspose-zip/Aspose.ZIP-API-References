---
title: "Classe LhaArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Lha.LhaArchive. Questa classe rappresenta un file archivio LHA .lzh"
type: docs
weight: 630
url: /it/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Questa classe rappresenta un file di archivio LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Inizializza una nuova istanza della classe `LhaArchive` e compone un elenco di voci che possono essere estratte dall'archivio. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Inizializza una nuova istanza della classe `LhaArchive` e compone un elenco di voci che possono essere estratte dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Restituisce le voci file di tipo [`LhaArchiveEntry`](../lhaarchiveentry/) che costituiscono l'archivio. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Estrae tutti i file e le directory nell'archivio nella directory fornita. |

## Osservazioni

Sono supportati solo i seguenti metodi di compressione:

**Method**

**Explanation**

**lh0**

Non compresso

**lh4**

Dizionario scorrevole da 8 KiB e Huffman statico

**lh5**

Dizionario scorrevole da 16 KiB e Huffman statico

**lh6**

Dizionario scorrevole da 64 KiB e Huffman statico

**lh7**

Dizionario scorrevole da 128 KiB e Huffman statico

**lhx**

Dizionario scorrevole da 1 Mib e Huffman statico

**lhd**

Cartella

### Vedi anche

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


