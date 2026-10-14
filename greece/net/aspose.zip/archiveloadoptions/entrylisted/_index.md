---
title: "ArchiveLoadOptions.EntryListed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα ArchiveLoadOptions. Λαμβάνει ή ορίζει τον delegate που καλείται όταν μια καταχώρηση εμφανίζεται στον πίνακα περιεχομένων"
type: docs
weight: 60
url: /el/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Λαμβάνει ή ορίζει τον αντιπρόσωπο που καλείται όταν μια καταχώρηση εμφανίζεται στον πίνακα περιεχομένων.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

## Παραδείγματα

```csharp
var archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Δείτε επίσης

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


