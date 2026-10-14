---
title: "FastLZStream.FastLZStream"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Costruttore FastLZStream. Inizializza una nuova istanza della classe FastLZStream preparata per la compressione"
type: docs
weight: 10
url: /it/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Inizializza una nuova istanza della classe [`FastLZStream`](../) preparata per la compressione.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | Il flusso per salvare i dati compressi. |
| compressionLevel | Int32 | Usa 1 per una compressione più veloce, usa 2 per un rapporto di compressione migliore. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | *stream* è nullo. |
| ArgumentException | *stream* non supporta la scrittura. |
| ArgumentOutOfRangeException | *compressionLevel* è maggiore di 2 o minore di 1. |

### Vedi anche

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


