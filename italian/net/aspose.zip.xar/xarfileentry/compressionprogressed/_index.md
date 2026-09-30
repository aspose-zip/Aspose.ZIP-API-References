---
title: "XarFileEntry.CompressionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento XarFileEntry. Viene sollevato quando una porzione di flusso grezzo è compressa"
type: docs
weight: 20
url: /it/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Viene sollevata quando una parte del flusso grezzo è compressa.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Osservazioni

Il mittente dell'evento è un'istanza [`XarFileEntry`](../).

## Esempi

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


