---
title: "ArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Event ArchiveEntry. Dipicu ketika sebagian aliran mentah telah diekstrak"
type: docs
weight: 100
url: /id/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Dipicu ketika sebagian aliran mentah diekstrak.

```csharp
public event EventHandler<ProgressCancelEventArgs> ExtractionProgressed;
```

## Catatan

Pengirim event adalah sebuah instance [`ArchiveEntry`](../). Dimungkinkan untuk membatalkan ekstraksi.

## Contoh

Dalam contoh ini, penangan acara digunakan untuk menghitung bagian ukuran yang diproses dalam persen.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

Dalam contoh ini, penangan acara digunakan untuk pembatalan setelah seratus Mb pertama dari entri diekstrak.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => { if (e.ProceededBytes > 100000000) e.Cancel = true; };
```

### Lihat Juga

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


