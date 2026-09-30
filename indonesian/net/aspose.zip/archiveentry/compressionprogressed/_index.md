---
title: "ArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Acara ArchiveEntry. Dipicu ketika sebagian aliran mentah dikompresi"
type: docs
weight: 90
url: /id/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

Dipicu ketika sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Catatan

Pengirim acara adalah sebuah instance [`ArchiveEntry`](../).

## Contoh

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat Juga

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


