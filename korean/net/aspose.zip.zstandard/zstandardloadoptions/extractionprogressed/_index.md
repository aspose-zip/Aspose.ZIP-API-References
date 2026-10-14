---
title: "ZstandardLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ZstandardLoadOptions 이벤트. 일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.zstandard/zstandardloadoptions/extractionprogressed/
---
## ZstandardLoadOptions.ExtractionProgressed event

일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 비고

이벤트 발신자는 추출이 진행 중인 [`ZstandardArchive`](../../zstandardarchive/) 인스턴스입니다.

## 예제

```csharp
ZstandardArchive archive = new ZstandardArchive("archive.zst", 
new ZStandardLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZstandardLoadOptions](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardloadoptions/)
* assembly [Aspose.Zip](../../../)


