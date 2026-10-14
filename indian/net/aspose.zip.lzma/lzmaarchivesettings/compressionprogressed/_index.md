---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "LzmaArchiveSettings इवेंट। जब कच्ची स्ट्रीम का एक भाग संकुचित हो जाता है तो उठाया जाता है"
type: docs
weight: 50
url: /hi/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है तो उत्पन्न होता है।

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## उदाहरण

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


