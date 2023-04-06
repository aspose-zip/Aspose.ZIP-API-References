---
title: Class ParallelOptions
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Saving.ParallelOptions 수업. 병렬 압축 옵션.
type: docs
weight: 490
url: /ko/net/aspose.zip.saving/paralleloptions/
---
## ParallelOptions class

병렬 압축 옵션.

```csharp
public class ParallelOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ParallelOptions](paralleloptions/)() | 기본 생성자입니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [AvailableMemorySize](../../aspose.zip.saving/paralleloptions/availablememorysize/) { get; set; } | 디스크로 스왑하지 않고 압축된 항목을 수용하는 데 사용할 수 있는 메모리 추정치를 메가바이트 단위로 가져오거나 설정합니다. 이 값은 다음과 같은 경우에만 의미가 있습니다.[`ParallelCompressInMemory`](./parallelcompressinmemory/) 설정이 있습니다Auto 모드. |
| [ParallelCompressInMemory](../../aspose.zip.saving/paralleloptions/parallelcompressinmemory/) { get; set; } | 병렬 접근 방법을 나타내는 값을 가져오거나 설정합니다. |

### 비고

이 옵션은 여러 CPU 코어에 의한 동시 압축을 관리합니다.

### 예

```csharp
using (var archive = new Archive())
{
    archive.CreateEntries("DirToCompress");
    archive.Save("archive.zip", new ArchiveSaveOptions() { ParallelOptions = new ParallelOptions { ParallelCompressInMemory = mode, AvailableMemorySize = 4000 } });
}
```

### 또한보십시오

* 네임스페이스 [Aspose.Zip.Saving](../../aspose.zip.saving/)
* 집회 [Aspose.Zip](../../)


