---
title: "ZArchiveLoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ZArchiveLoadOptions 이벤트. 일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.zip.z/zarchiveloadoptions/extractionprogressed/
---
## ZArchiveLoadOptions.ExtractionProgressed event

일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 비고

이벤트 발신자는 추출이 진행 중인 [`ZArchive`](../../zarchive/) 인스턴스입니다.

## 예제

```csharp
ZArchive archive = new ZArchive("archive.z", 
new ZArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


