---
title: "XarFileEntry.CompressionProgressed"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "حدث XarFileEntry. يُثار عندما يتم ضغط جزء من تدفق البيانات الخام"
type: docs
weight: 20
url: /ar/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

يُرفع عندما يتم ضغط جزء من تدفق البيانات الخام.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## ملاحظات

مرسل الحدث هو كائن [`XarFileEntry`](../).

## أمثلة

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### انظر أيضًا

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


