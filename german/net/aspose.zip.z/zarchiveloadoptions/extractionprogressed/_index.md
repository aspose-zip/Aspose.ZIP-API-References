---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZArchiveLoadOptions-Ereignis. Ruft den Delegaten ab oder legt ihn fest, der aufgerufen wird, wenn einige Bytes extrahiert wurden"
type: docs
weight: 30
url: /de/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Liest oder setzt den Delegaten, der aufgerufen wird, wenn einige Bytes extrahiert wurden.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Hinweise

Der Ereignisabsender ist die [`ZArchive`](../../zarchive/)‑Instanz, bei der die Extraktion fortschreitet.

## Beispiele

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


