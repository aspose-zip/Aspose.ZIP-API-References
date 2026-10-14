---
title: "SevenZipArchiveEntry.CompressionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Event SevenZipArchiveEntry. Dikeluarkan ketika sebagian aliran mentah terkompresi"
type: docs
weight: 70
url: /id/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

Dipicu ketika sebagian aliran mentah dikompresi.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Catatan

Pengirim event adalah sebuah instance [`SevenZipArchiveEntry`](../).

Tidak dipanggil dalam mode solid dan mode multithread untuk entri LZMA2.

## Contoh

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


