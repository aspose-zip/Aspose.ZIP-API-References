---
title: Class SevenZipLZMACompressionSettings
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Saving.SevenZipLZMACompressionSettings classe. Impostazioni per il metodo di compressione LZMA allinterno dellarchivio 7z.
type: docs
weight: 580
url: /it/net/aspose.zip.saving/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings class

Impostazioni per il metodo di compressione LZMA all'interno dell'archivio 7z.

```csharp
public class SevenZipLZMACompressionSettings : SevenZipCompressionSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SevenZipLZMACompressionSettings](sevenziplzmacompressionsettings/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DictionarySize](../../aspose.zip.saving/sevenziplzmacompressionsettings/dictionarysize/) { get; set; } | La dimensione del dizionario (buffer storico) indica quanti byte dei dati non compressi elaborati di recente sono conservati in memoria. Se non impostato, verrà scelto in base alla dimensione della voce. |
| override [Method](../../aspose.zip.saving/sevenziplzmacompressionsettings/method/) { get; } | Ottiene il metodo di compressione o decompressione. |

### Osservazioni

L'algoritmo della catena Lempel-Ziv-Markov (LZMA) è un algoritmo utilizzato per eseguire la compressione dei dati senza perdita. Questo algoritmo utilizza uno schema di compressione del dizionario in qualche modo simile all'algoritmo LZ77 e presenta un rapporto di compressione elevato e una dimensione del dizionario di compressione variabile.

Per saperne di più: https://en.wikipedia.org/wiki/Lempel–Ziv–Markov_chain_algorithm

### Guarda anche

* class [SevenZipCompressionSettings](../sevenzipcompressionsettings/)
* spazio dei nomi [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assemblea [Aspose.Zip](../../)


