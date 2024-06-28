---
title: ArchiveLoadOptions.EntryListed
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveLoadOptions property. Gets or sets the delegate invoked when an entry listed within table of content
type: docs
weight: 50
url: /net/aspose.zip/archiveloadoptions/entrylisted/
---
## ArchiveLoadOptions.EntryListed property

Gets or sets the delegate invoked when an entry listed within table of content.

```csharp
public EventHandler<EntryEventArgs> EntryListed { get; set; }
```

## Examples

```csharp
Archive archive = new Archive("archive.zip", new ArchiveLoadOptions() { EntryListed = (s, e) => { Console.WriteLine(e.Entry.Name); } });
```

### See Also

* class [EntryEventArgs](../../entryeventargs/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


