---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Bzip2SaveOptions-händelsen. Utlöser när en del av den råa strömmen har komprimerats"
type: docs
weight: 40
url: /sv/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

Utlöser när en del av den råa strömmen komprimeras.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## Anmärkningar

Denna händelse kommer inte att utlösas när komprimering sker i flerdelat läge.

## Exempel

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### Se även

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


