---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveLoadOptions Properti. Mendapat atau menyetel delegasi yang dipanggil saat entri tercantum dalam daftar isi.
type: docs
weight: 50
url: /id/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Mendapat atau menyetel delegasi yang dipanggil saat entri tercantum dalam daftar isi.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Contoh

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Lihat juga

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* ruang nama [Aspose.Zip](../../archiveloadoptions/)
* perakitan [Aspose.Zip](../../../)


