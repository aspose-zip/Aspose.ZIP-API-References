---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: Aspose.ZIP für .NET-API-Referenz
description: ArchiveLoadOptions eigendom. Ruft den Delegaten ab oder legt ihn fest der aufgerufen wird wenn einige Bytes extrahiert wurden.
type: docs
weight: 40
url: /de/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

Ruft den Delegaten ab oder legt ihn fest, der aufgerufen wird, wenn einige Bytes extrahiert wurden.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### Bemerkungen

Absender des Ereignisses ist der[`ArchiveEntry`](../../archiveentry/) Instanz, welche Extraktion vorangetrieben wird.

### Beispiele

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### Siehe auch

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* namensraum [Aspose.Zip](../../archiveloadoptions/)
* Montage [Aspose.Zip](../../../)


