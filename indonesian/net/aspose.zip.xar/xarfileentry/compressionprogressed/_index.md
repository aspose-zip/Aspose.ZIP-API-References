---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "XarFileEntry event. Dipicu ketika sebagian aliran mentah terkompresi"
type: docs
weight: 20
url: /id/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

Dipicu ketika sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Catatan

Pengirim event adalah sebuah instance [`XarFileEntry`](../).

## Contoh

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


