---
title: "ArchiveLoadOptions.EntryListed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti ArchiveLoadOptions. Mendapatkan atau mengatur delegasi yang dipanggil ketika sebuah entri terdaftar dalam daftar isi"
type: docs
weight: 60
url: /id/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Mendapatkan atau mengatur delegasi yang dipanggil ketika sebuah entri terdaftar dalam tabel konten.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

## Contoh

```csharp
var archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Lihat Juga

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


