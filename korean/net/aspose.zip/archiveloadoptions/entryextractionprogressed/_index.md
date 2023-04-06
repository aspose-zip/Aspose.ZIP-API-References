---
title: ArchiveLoadOptions.EntryExtractionProgressed
second_title: .NET API 참조용 Aspose.ZIP
description: ArchiveLoadOptions 재산. 일부 바이트가 추출되었을 때 호출되는 대리자를 가져오거나 설정합니다.
type: docs
weight: 40
url: /ko/net/aspose.zip/archiveloadoptions/entryextractionprogressed/
---
## ArchiveLoadOptions.EntryExtractionProgressed property

일부 바이트가 추출되었을 때 호출되는 대리자를 가져오거나 설정합니다.

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

### 비고

이벤트 발신자는[`ArchiveEntry`](../../archiveentry/) 추출이 진행되는 인스턴스.

### 예

```csharp
Archive archive = new Archive("archive.zip", 
new ArchiveLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); } })                 
```

### 또한보십시오

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveLoadOptions](../)
* 네임스페이스 [Aspose.Zip](../../archiveloadoptions/)
* 집회 [Aspose.Zip](../../../)


