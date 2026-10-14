---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Event Bzip2SaveOptions. Dipicu ketika sebagian aliran mentah dikompresi."
type: docs
weight: 40
url: /id/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Dipicu ketika sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Catatan

Event ini tidak akan dipicu saat melakukan kompresi dalam mode multithread.

## Contoh

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


