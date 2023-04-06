---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveLoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει τον εκπρόσωπο που καλείται όταν μια καταχώριση παρατίθεται στον πίνακα περιεχομένου.
type: docs
weight: 50
url: /el/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Λαμβάνει ή ορίζει τον εκπρόσωπο που καλείται όταν μια καταχώριση παρατίθεται στον πίνακα περιεχομένου.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Παραδείγματα

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Δείτε επίσης

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveloadoptions/)
* συνέλευση [Aspose.Zip](../../../)


