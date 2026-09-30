---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarFileEntry इवेंट। जब कच्ची स्ट्रीम का एक भाग संकुचित हो जाता है तो उठाया जाता है"
type: docs
weight: 20
url: /hi/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

जब कच्ची स्ट्रीम का एक भाग संकुचित किया जाता है तो उत्पन्न होता है।

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## टिप्पणियाँ

इवेंट प्रेषक एक [`XarFileEntry`](../) इंस्टेंस है।

## उदाहरण

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


