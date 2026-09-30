---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Peristiwa LzmaArchiveSettings. Dibangkitkan ketika sebagian aliran mentah dikompresi"
type: docs
weight: 50
url: /id/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

Dipicu ketika sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Contoh

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


