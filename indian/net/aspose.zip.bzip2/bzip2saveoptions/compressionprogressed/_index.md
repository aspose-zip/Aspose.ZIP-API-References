---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "Bzip2SaveOptions इवेंट। जब कच्ची स्ट्रीम का एक भाग संकुचित होता है, तब उठाया जाता है"
type: docs
weight: 40
url: /hi/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है तो उत्पन्न होता है।

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## टिप्पणियाँ

जब मल्टीथ्रेडेड मोड में संकुचन किया जाता है, तो यह इवेंट नहीं उठाया जाएगा।

## उदाहरण

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


