---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZstandardLoadOptions-händelse. Hämtar eller anger delegaten som anropas när några byte har extraherats"
type: docs
weight: 30
url: /sv/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

Hämtar eller anger delegaten som anropas när några byte har extraherats.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Anmärkningar

Händelseavsändaren är [`ZstandardArchive`](../../zstandardarchive/) instansen vars extraktion har fortskridit.

## Exempel

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


