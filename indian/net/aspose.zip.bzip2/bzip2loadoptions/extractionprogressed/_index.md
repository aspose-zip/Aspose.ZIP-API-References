---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Bzip2LoadOptions इवेंट। जब कुछ बाइट्स निकाले जा चुके हों तो इवेंट उठाया जाता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

जब कुछ बाइट्स निकाले जा चुके हों तो उठाया गया इवेंट सक्रिय होता है।

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## टिप्पणियाँ

इवेंट प्रेषक वह [`Bzip2Archive`](../../bzip2archive/) इंस्टेंस है जिसका निष्कर्षण प्रगति पर है। [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/) वह बाइट्स की संख्या है जो निष्कर्षण के बाद है।

## उदाहरण

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


