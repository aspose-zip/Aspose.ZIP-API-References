---
title: "ZstandardSaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ZstandardSaveOptions 이벤트. 원시 스트림의 일부가 압축될 때 발생합니다."
type: docs
weight: 20
url: /ko/net/aspose.zip.zstandard/zstandardsaveoptions/compressionprogressed/
---
## ZstandardSaveOptions.CompressionProgressed event

원시 스트림의 일부가 압축될 때 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 예제

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardSaveOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardsaveoptions/)
* assembly [Aspose.Zip](../../../)


