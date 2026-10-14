---
title: "RarArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Acara RarArchiveEntry. Diumumkan ketika sebagian aliran mentah diekstrak"
type: docs
weight: 80
url: /id/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

Dipicu ketika sebagian aliran mentah diekstrak.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Catatan

Pengirim acara adalah sebuah instance [`RarArchiveEntry`](../).

## Contoh

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


