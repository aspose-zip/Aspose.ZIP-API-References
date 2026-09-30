---
title: "XarLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarLoadOptions 속성. 일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다"
type: docs
weight: 30
url: /ko/net/aspose.zip.xar/xarloadoptions/entryextractionprogressed/
---
## XarLoadOptions.EntryExtractionProgressed property

일부 바이트가 추출될 때 호출되는 대리자를 가져오거나 설정합니다.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## 비고

이벤트 발신자는 추출이 진행 중인 [`XarFileEntry`](../../xarfileentry/) 인스턴스입니다.

## 예제

```csharp
XarArchive archive = new XarArchive("archive.xar", 
new XarLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((XarFileEntry)s).Length); } })                 
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


