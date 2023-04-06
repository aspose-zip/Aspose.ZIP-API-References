---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: PPMdCompressionSettings 건설자. 의 새 인스턴스를 초기화합니다.PPMdCompressionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`PPMdCompressionSettings`](../) 클래스.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| modelOrder | Int32 | 모델의 순서. |
| suballocatorSize | Int32 | MB 하위 할당자의 메모리 크기가 소모될 수 있습니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* 2와 16 사이가 아닙니다. - 또는 -*suballocatorSize* 1에서 256 사이가 아닙니다. |

### 비고

더 큰 모델 주문은 거의 확실하게 더 나은 압축과 더 많은 메모리 및 CPU 사용량을 초래합니다.

PPMd 알고리즘은 특히 큰 파일에 사용하거나 큰 모델 순서와 함께 사용할 때 많은 메모리가 필요할 수 있습니다.

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [PPMdCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

의 새 인스턴스를 초기화합니다.[`PPMdCompressionSettings`](../) 기본 모델 순서 및 하위 할당자 크기가 있는 클래스.

```csharp
public PPMdCompressionSettings()
```

### 비고

기본 모델 순서는 8이고 하위 할당자 크기는 50MB입니다.

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [PPMdCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* 집회 [Aspose.Zip](../../../)


