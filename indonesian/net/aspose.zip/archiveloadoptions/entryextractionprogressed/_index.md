---
title: "ArchiveLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti ArchiveLoadOptions. Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak"
type: docs
weight: 50
url: /id/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Mendapatkan atau mengatur delegasi yang dipanggil ketika beberapa byte telah diekstrak.

```csharp
public EventHandler<ProgressCancelEventArgs> EntryExtractionProgressed { get; set; }
```

## Catatan

Pengirim acara adalah instance [`ArchiveEntry`](../../archiveentry/) yang ekstraksinya sedang diproses.

## Contoh

Lacak kemajuan ekstraksi sebuah entri.

```csharp
var archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

Batalkan ekstraksi entri setelah waktu tertentu.

```csharp
Stopwatch watch = Stopwatch.StartNew();
using (Archive a = new Archive("big.zip", new ArchiveLoadOptions() {
    EntryExtractionProgressed = (s, e) => { if (watch.ElapsedMilliseconds > 1000) e.Cancel = true; } }))
{
    a.Entries[0].Extract("first.bin");
}
```

### Lihat Juga

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


