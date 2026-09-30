---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento ZArchiveSaveOptions. Viene generato quando una porzione del flusso grezzo viene compressa"
type: docs
weight: 20
url: /it/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

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
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


