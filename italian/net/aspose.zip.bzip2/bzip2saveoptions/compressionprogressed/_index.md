---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento Bzip2SaveOptions. Viene sollevato quando una parte del flusso grezzo è compressa"
type: docs
weight: 40
url: /it/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Viene sollevata quando una parte del flusso grezzo è compressa.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Osservazioni

Questo evento non verrà sollevato quando si comprime in modalità multithread.

## Esempi

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


