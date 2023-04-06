---
title: ParallelOptions.AvailableMemorySize
second_title: .NET API 참조용 Aspose.ZIP
description: ParallelOptions 재산. 디스크로 스왑하지 않고 압축된 항목을 수용하는 데 사용할 수 있는 메모리 추정치를 메가바이트 단위로 가져오거나 설정합니다. 이 값은 다음과 같은 경우에만 의미가 있습니다.ParallelCompressInMemory 설정이 있습니다Auto 모드.
type: docs
weight: 20
url: /ko/net/aspose.zip.saving/paralleloptions/availablememorysize/
---
## ParallelOptions.AvailableMemorySize property

디스크로 스왑하지 않고 압축된 항목을 수용하는 데 사용할 수 있는 메모리 추정치를 메가바이트 단위로 가져오거나 설정합니다. 이 값은 다음과 같은 경우에만 의미가 있습니다.[`ParallelCompressInMemory`](../parallelcompressinmemory/) 설정이 있습니다Auto 모드.

```csharp
public int AvailableMemorySize { get; set; }
```

### 비고

이 값은 다른 항목과 병렬로 압축할 수 있는 항목의 최대 크기를 계산하는 데 사용됩니다. 계산된 임계값을 초과하는 모든 항목은 순차적으로 압축됩니다. `AvailableMemorySize` 무료 RAM만큼 크고 더 큰 재산. 기본적으로 CPU 코어당 최소 200MB가 있다고 가정합니다.

### 또한보십시오

* class [ParallelOptions](../)
* 네임스페이스 [Aspose.Zip.Saving](../../paralleloptions/)
* 집회 [Aspose.Zip](../../../)


