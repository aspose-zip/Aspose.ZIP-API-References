---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "XarLoadOptions-Eigenschaft. Liest oder setzt den Delegaten, der aufgerufen wird, wenn einige Bytes extrahiert wurden."
type: docs
weight: 30
url: /de/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Liest oder setzt den Delegaten, der aufgerufen wird, wenn einige Bytes extrahiert wurden.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Hinweise

Der Ereignisabsender ist die [`XarFileEntry`](../../xarfileentry/) Instanz, deren Extraktion fortschreitet.

## Beispiele

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


