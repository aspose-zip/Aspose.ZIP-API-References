---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti XarLoadOptions. Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak."
type: docs
weight: 30
url: /id/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Catatan

Pengirim peristiwa adalah instance [`XarFileEntry`](../../xarfileentry/) yang proses ekstraksinya sedang berlangsung.

## Contoh

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


