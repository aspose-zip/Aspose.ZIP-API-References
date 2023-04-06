---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveLoadOptions mülk. İçindekiler tablosunda bir giriş listelendiğinde çağrılan temsilciyi alır veya ayarlar.
type: docs
weight: 50
url: /tr/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

İçindekiler tablosunda bir giriş listelendiğinde çağrılan temsilciyi alır veya ayarlar.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Örnekler

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Ayrıca bakınız

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* ad alanı [Aspose.Zip](../../archiveloadoptions/)
* toplantı [Aspose.Zip](../../../)


