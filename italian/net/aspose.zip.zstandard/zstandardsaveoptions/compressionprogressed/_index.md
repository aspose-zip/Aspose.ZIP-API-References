---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento ZstandardSaveOptions. Viene sollevato quando una porzione di flusso grezzo è compressa"
type: docs
weight: 20
url: /it/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

Viene sollevata quando una parte del flusso grezzo è compressa.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Esempi

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


