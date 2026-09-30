---
title: "Bzip2SaveOptions.CompressionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Bzip2SaveOptions 이벤트. 원시 스트림의 일부가 압축될 때 발생합니다."
type: docs
weight: 40
url: /ko/net/aspose.zip.bzip2/bzip2saveoptions/compressionprogressed/
---
## Bzip2SaveOptions.CompressionProgressed event

원시 스트림의 일부가 압축될 때 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

## 비고

멀티스레드 모드에서 압축할 때는 이 이벤트가 발생하지 않습니다.

## 예제

```csharp
settings.CompressionProgressed += (s, e) => { int percent = (int)((100 * e.ProceededBytes) / entrySourceStream.Length); };
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


