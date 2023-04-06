---
title: Class ParallelOptions
second_title: Riferimento API Aspose.ZIP per .NET
description: Aspose.Zip.Saving.ParallelOptions classe. Opzioni per la compressione parallela.
type: docs
weight: 490
url: /it/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

Opzioni per la compressione parallela.

```csharp
public class ParallelOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | Ottiene o imposta la stima della memoria in megabyte disponibile per accogliere voci compresse senza swap su disco. Questo valore ha senso solo se[`ParallelCompressInMemory`](./parallelcompressinmemory/) l'impostazione è inAuto modalità. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | Ottiene o imposta il valore che indica come utilizzare l'approccio parallelo. |

### Osservazioni

Queste opzioni gestiscono la compressione simultanea di più core della CPU.

### Esempi

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### Guarda anche

* spazio dei nomi [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assemblea [Aspose.Zip](../../)


