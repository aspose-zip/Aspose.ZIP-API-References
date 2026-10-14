---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "ZstandardLoadOptions peristiwa. Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak."
type: docs
weight: 30
url: /id/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Catatan

Pengirim peristiwa adalah instance [`ZstandardArchive`](../../zstandardarchive/) yang ekstraksinya sedang berlangsung.

## Contoh

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


