---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Riferimento API Aspose.ZIP per .NET"
description: "Evento Bzip2LoadOptions. Evento sollevato quando alcuni byte sono stati estratti"
type: docs
weight: 30
url: /it/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Evento generato quando alcuni byte sono stati estratti.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Osservazioni

Il mittente dell'evento è l'istanza [`Bzip2Archive`](../../bzip2archive/) la cui estrazione è in corso. Il [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) è il numero di byte dopo l'estrazione.

## Esempi

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Vedi anche

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


