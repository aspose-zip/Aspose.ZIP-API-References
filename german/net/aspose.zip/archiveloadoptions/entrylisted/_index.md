---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveLoadOptions eigendom. Ruft den Delegaten ab oder legt ihn fest der aufgerufen wird wenn ein Eintrag im Inhaltsverzeichnis aufgeführt wird.
type: docs
weight: 50
url: /de/net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Ruft den Delegaten ab oder legt ihn fest, der aufgerufen wird, wenn ein Eintrag im Inhaltsverzeichnis aufgeführt wird.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

### Beispiele

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### Siehe auch

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* namensraum [Aspose.Zip](../../archiveloadoptions/)
* Montage [Aspose.Zip](../../../)


