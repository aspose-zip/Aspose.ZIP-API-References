---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "ZArchiveLoadOptions händelse. Hämtar eller anger delegaten som anropas när några byte har extraherats"
type: docs
weight: 30
url: /sv/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

Hämtar eller anger delegaten som anropas när några byte har extraherats.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Anmärkningar

Evenemangsavsändaren är [`ZArchive`](../../zarchive/)-instansen vars extraktion har fortskridit.

## Exempel

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


