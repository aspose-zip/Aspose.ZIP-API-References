---
title: "LzmaArchiveSettings.CompressionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "LzmaArchiveSettings 이벤트. 원시 스트림의 일부가 압축될 때 발생합니다"
type: docs
weight: 50
url: /ko/net/aspose.zip.lzma/lzmaarchivesettings/compressionprogressed/
---
## LzmaArchiveSettings.CompressionProgressed event

원시 스트림의 일부가 압축될 때 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 예제

```csharp
lzmaArchiveSettings.CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


