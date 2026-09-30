---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "Bzip2LoadOptions olayı. Bazı baytlar çıkarıldığında tetiklenen olay"
type: docs
weight: 30
url: /tr/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

Bazı baytlar çıkarıldığında tetiklenen olay.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## Açıklamalar

Olay göndericisi, çıkarma işlemi ilerleyen [`Bzip2Archive`](../../bzip2archive/) örneğidir. [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) ise çıkarma sonrası bayt sayısını belirtir.

## Örnekler

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### Ayrıca Bakınız

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


