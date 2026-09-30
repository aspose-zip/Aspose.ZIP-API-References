---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Event Bzip2LoadOptions. Event yang dipicu ketika sejumlah byte telah diekstrak."
type: docs
weight: 30
url: /id/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Peristiwa yang dipicu ketika beberapa byte telah diekstrak.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Catatan

Pengirim event adalah instance [`Bzip2Archive`](../../bzip2archive/) yang ekstraksinya sedang berlangsung. [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) adalah jumlah byte setelah ekstraksi.

## Contoh

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Lihat Juga

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


