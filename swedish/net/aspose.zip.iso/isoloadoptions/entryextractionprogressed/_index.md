---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoLoadOptions egenskap. Hämtar eller anger delegaten som anropas när några byte har extraherats"
type: docs
weight: 30
url: /sv/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

Hämtar eller anger delegaten som anropas när några byte har extraherats.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Anmärkningar

Evenemangsavsändaren är [`IsoEntry`](../../isoentry/)-instansen vars extraktion har fortskridit.

## Exempel

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


