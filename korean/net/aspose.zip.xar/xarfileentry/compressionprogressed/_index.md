---
title: "XarFileEntry.CompressionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarFileEntry 이벤트. 원시 스트림의 일부가 압축될 때 발생합니다"
type: docs
weight: 20
url: /ko/net/aspose.zip.xar/xarfileentry/compressionprogressed/
---
## XarFileEntry.CompressionProgressed event

원시 스트림의 일부가 압축될 때 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 비고

이벤트 발신자는 [`XarFileEntry`](../) 인스턴스입니다.

## 예제

```csharp
archive.Entries.First().CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarFileEntry](../)
* namespace [Aspose.Zip.Xar](../../xarfileentry/)
* assembly [Aspose.Zip](../../../)


