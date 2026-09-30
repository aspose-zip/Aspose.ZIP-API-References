---
title: "Classe ArjArchive"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Classe Aspose.Zip.Arj.ArjArchive. Questa classe rappresenta un file di archivio ARJ"
type: docs
weight: 250
url: /it/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

Questa classe rappresenta un file di archivio ARJ.

```csharp
public class ArjArchive : IArchive
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | Inizializza una nuova istanza della classe `ArjArchive` e compone un elenco di voci che può essere estratto dall'archivio. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | Inizializza una nuova istanza della classe `ArjArchive` e compone un elenco di voci che può essere estratto dall'archivio. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | Ottiene il commento. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | Ottiene le voci di tipo [`ArjEntryPlain`](../arjentryplain/) che costituiscono l'archivio ARJ. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | Ottiene il nome originale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | Esegue operazioni definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | Estrae tutte le voci nella directory specificata. |

## Osservazioni

Sono supportati solo i seguenti metodi di compressione:

**Method**

**Explanation**

**0**

Non compresso

**1**

Combinazione di LZ77 e codifica Huffman adattiva. Rapporto migliore.

**2**

Combinazione di LZ77 e codifica Huffman adattiva.

**3**

Combinazione di LZ77 e codifica Huffman adattiva. Velocità migliore.

### Vedi anche

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


