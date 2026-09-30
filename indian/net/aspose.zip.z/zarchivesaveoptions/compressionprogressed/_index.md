---
title: "ZArchiveSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "ZArchiveSaveOptions इवेंट। जब कच्ची स्ट्रीम का एक भाग संकुचित हो तो उठाया जाता है"
type: docs
weight: 20
url: /hi/net/aspose.zip.z/zarchivesaveoptions/compressionprogressed/
---
## ZArchiveSaveOptions.CompressionProgressed event

जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है तो उत्पन्न होता है।

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## उदाहरण

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveSaveOptions](../)
* namespace [Aspose.Zip.Z](../../zarchivesaveoptions/)
* assembly [Aspose.Zip](../../../)


