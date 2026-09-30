---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث Bzip2LoadOptions. الحدث يُثار عندما يتم استخراج بعض البايتات"
type: docs
weight: 30
url: /ar/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

الحدث الذي يُرفع عند استخراج بعض البايتات.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## ملاحظات

مرسل الحدث هو الكائن [`Bzip2Archive`](../../bzip2archive/) الذي يتم فيه تقدم الاستخراج. الـ[`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) هو عدد البايتات بعد الاستخراج.

## أمثلة

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


