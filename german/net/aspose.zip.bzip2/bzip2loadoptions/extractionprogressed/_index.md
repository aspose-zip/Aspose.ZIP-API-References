---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "Bzip2LoadOptions Ereignis. Ereignis wird ausgelöst, wenn einige Bytes extrahiert wurden."
type: docs
weight: 30
url: /de/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Ereignis, das ausgelöst wird, wenn einige Bytes extrahiert wurden.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Hinweise

Der Ereignisabsender ist die [`Bzip2Archive`](../../bzip2archive/) Instanz, deren Extraktion fortgeschritten ist. Das [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) ist die Anzahl der Bytes nach der Extraktion.

## Beispiele

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Siehe auch

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


