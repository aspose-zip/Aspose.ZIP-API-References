---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Bzip2LoadOptions händelse. Händelse som utlöses när vissa byte har extraherats"
type: docs
weight: 30
url: /sv/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Händelse som utlöses när några byte har extraherats.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Anmärkningar

Avsändaren av händelsen är [`Bzip2Archive`](../../bzip2archive/)‑instansen vars extraktion har fortskridit. [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) är antalet byte efter extraktionen.

## Exempel

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


