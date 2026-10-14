---
title: "Bzip2LoadOptions.ExtractionProgressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Bzip2LoadOptions 이벤트. 일부 바이트가 추출될 때 발생하는 이벤트"
type: docs
weight: 30
url: /ko/net/aspose.zip.bzip2/bzip2loadoptions/extractionprogressed/
---
## Bzip2LoadOptions.ExtractionProgressed event

일부 바이트가 추출될 때 발생하는 이벤트.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

## 비고

이벤트 발신자는 추출이 진행 중인 [`Bzip2Archive`](../../bzip2archive/) 인스턴스입니다. [`ProceededBytes`](../../../aspose.zip/progresseventargs/proceededbytes/)는 추출 후의 바이트 수입니다.

## 예제

```csharp
Bzip2LoadOptions loadOptions = new Bzip2LoadOptions(); 
loadOptions.ExtractionProgressed += (s, e) => { percent = (int) ((double)(100 * e.ProceededBytes) / originalFileLength); };
```

### 또 보기

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [Bzip2LoadOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2loadoptions/)
* assembly [Aspose.Zip](../../../)


