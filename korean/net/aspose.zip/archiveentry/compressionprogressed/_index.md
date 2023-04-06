---
title: ArchiveEntry.CompressionProgressed
second_title: .NET API 참조용 Aspose.ZIP
description: ArchiveEntry 이벤트. 원시 스트림의 일부가 압축되면 발생합니다.
type: docs
weight: 80
url: /ko/net/aspose.zip/archiveentry/compressionprogressed/
---
## ArchiveEntry.CompressionProgressed event

원시 스트림의 일부가 압축되면 발생합니다.

```csharp
public event EventHandler<ProgressEventArgs> CompressionProgressed;
```

### 비고

이벤트 발신자는[`ArchiveEntry`](../) 사례.

### 예

```csharp
archive.Entries[0].CompressionProgressed += (s, e) => { int percent = (int)((100 * (long)e.ProceededBytes) / entrySourceStream.Length); };
```

### 또한보십시오

* class [ProgressEventArgs](../../progresseventargs/)
* class [ArchiveEntry](../)
* 네임스페이스 [Aspose.Zip](../../archiveentry/)
* 집회 [Aspose.Zip](../../../)


