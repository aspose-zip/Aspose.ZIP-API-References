---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Event ZArchiveSaveOptions. Dikeluarkan ketika sebagian aliran mentah terkompresi"
type: docs
weight: 20
url: /id/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

Dipicu ketika sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Contoh

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


