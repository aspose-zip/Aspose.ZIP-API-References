---
title: SevenZipArchiveEntry.CompressionProgressed
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipArchiveEntry 이벤트. 원시 스트림의 일부가 압축되면 발생합니다.
type: docs
weight: 70
url: /ko/net/aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/
---
## SevenZipArchiveEntry.CompressionProgressed event

원시 스트림의 일부가 압축되면 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### 비고

이벤트 발신자는[`SevenZipArchiveEntry`](../) 사례.

### 예

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 또한보십시오

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [SevenZipArchiveEntry](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* 집회 [Aspose.Zip](../../../)


