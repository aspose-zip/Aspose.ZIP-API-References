---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "XarLoadOptions egenskap. Hämtar eller anger delegaten som anropas när några byte har extraherats"
type: docs
weight: 30
url: /sv/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

Hämtar eller anger delegaten som anropas när några byte har extraherats.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## Anmärkningar

Händelseavsändaren är [`XarFileEntry`](../../xarfileentry/)‑instansen vars extraktion har fortskridit.

## Exempel

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


