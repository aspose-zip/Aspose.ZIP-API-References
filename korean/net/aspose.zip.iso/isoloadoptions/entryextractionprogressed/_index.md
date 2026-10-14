---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoLoadOptions 속성. 일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## 비고

이벤트 발신자는 추출이 진행 중인 [`IsoEntry`](../../isoentry/) 인스턴스입니다.

## 예제

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


