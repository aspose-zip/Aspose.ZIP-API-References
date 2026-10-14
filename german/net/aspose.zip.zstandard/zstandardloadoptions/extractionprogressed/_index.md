---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "ZstandardLoadOptions-Ereignis. Gibt den Delegaten zurück oder legt ihn fest, der aufgerufen wird, wenn einige Bytes extrahiert wurden."
type: docs
weight: 30
url: /de/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Liest oder setzt den Delegaten, der aufgerufen wird, wenn einige Bytes extrahiert wurden.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Hinweise

Der Ereignisabsender ist die [`ZstandardArchive`](../../zstandardarchive/)‑Instanz, deren Extraktion fortschreitet.

## Beispiele

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


