---
title: ParallelOptions.AvailableMemorySize
second_title: Riferimento API Aspose.ZIP per .NET
description: ParallelOptions proprietà. Ottiene o imposta la stima della memoria in megabyte disponibile per accogliere voci compresse senza swap su disco. Questo valore ha senso solo seParallelCompressInMemory limpostazione è inAuto modalità.
type: docs
weight: 20
url: /it/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

Ottiene o imposta la stima della memoria in megabyte disponibile per accogliere voci compresse senza swap su disco. Questo valore ha senso solo se[`ParallelCompressInMemory`](../parallelcompressinmemory/) l'impostazione è inAuto modalità.

```csharp
public int AvailableMemorySize { get; set; }
```

### Osservazioni

Questo valore viene utilizzato per calcolare la dimensione massima della voce che può essere compressa in parallelo con altre. Tutte le voci al di sopra della soglia calcolata verranno compresse in sequenza. È sicuro averlo`AvailableMemorySize` proprietà grande quanto la RAM libera e anche più grande. Per impostazione predefinita si presume che tu abbia almeno 200 MB per core della CPU.

### Guarda anche

* class [ParallelOptions](../)
* spazio dei nomi [Aspose.Zip.Saving](../../paralleloptions/)
* assemblea [Aspose.Zip](../../../)


