---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "IsoLoadOptions Eigenschaft. Gibt den Aufrufdelegaten zurück oder setzt ihn, der aufgerufen wird, wenn einige Bytes extrahiert wurden."
type: docs
weight: 30
url: /de/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Liest oder setzt den Delegaten, der aufgerufen wird, wenn einige Bytes extrahiert wurden.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Hinweise

Der Ereignisabsender ist die [`IsoEntry`](../../isoentry/) Instanz, deren Extraktion fortschreitet.

## Beispiele

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


