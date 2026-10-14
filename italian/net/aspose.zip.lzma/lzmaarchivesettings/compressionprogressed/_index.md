---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento LzmaArchiveSettings. Viene sollevato quando una porzione del flusso grezzo viene compressa"
type: docs
weight: 50
url: /it/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Viene sollevata quando una parte del flusso grezzo è compressa.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Esempi

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


