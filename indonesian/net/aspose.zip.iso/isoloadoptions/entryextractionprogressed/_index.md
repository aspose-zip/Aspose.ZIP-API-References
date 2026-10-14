---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti IsoLoadOptions. Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak"
type: docs
weight: 30
url: /id/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Catatan

Pengirim acara adalah instansi [`IsoEntry`](../../isoentry/) yang sedang proses ekstraksinya.

## Contoh

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


