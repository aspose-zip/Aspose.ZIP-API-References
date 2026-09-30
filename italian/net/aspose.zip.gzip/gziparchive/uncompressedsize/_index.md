---
title: "GzipArchive.UncompressedSize"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Proprietà GzipArchive. Ottiene la dimensione di un file originale."
type: docs
weight: 30
url: /it/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Ottiene la dimensione di un file originale.

```csharp
public ulong UncompressedSize { get; }
```

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ObjectDisposedException | L'archivio è stato eliminato e non può essere utilizzato. |

## Osservazioni

Durante la decompressione, questa proprietà può contenere una dimensione errata. Se la dimensione del file decompressato supera i 4 GB, questa proprietà fornirà un valore sbagliato a causa del limite a 32 bit nell'intestazione.

### Vedi anche

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


