---
title: RarArchiveEntry.ExtractionProgressed
second_title: .NET API 참조용 Aspose.ZIP
description: RarArchiveEntry 이벤트. 원시 스트림의 일부가 추출되면 발생합니다.
type: docs
weight: 80
url: /ko/net/aspose.zip.rar/rararchiveentry/extractionprogressed/
---
## RarArchiveEntry.ExtractionProgressed event

원시 스트림의 일부가 추출되면 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> ExtractionProgressed;
```

### 비고

이벤트 발신자는[`RarArchiveEntry`](../) 사례.

### 예

```csharp
archive.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((RarArchiveEntry)s).UncompressedSize); };
```

### 또한보십시오

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [RarArchiveEntry](../)
* 네임스페이스 [Aspose.Zip.Rar](../../rararchiveentry/)
* 집회 [Aspose.Zip](../../../)


