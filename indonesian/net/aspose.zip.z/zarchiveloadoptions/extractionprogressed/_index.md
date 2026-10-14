---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Event ZArchiveLoadOptions. Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak"
type: docs
weight: 30
url: /id/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Catatan

Pengirim event adalah instance [`ZArchive`](../../zarchive/) yang proses ekstraksinya sedang berlangsung.

## Contoh

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


