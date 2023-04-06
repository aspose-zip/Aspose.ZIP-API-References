---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipPPMdCompressionSettings 건설자. 7z 아카이브 내에서 PPMd 압축 방법에 대한 설정을 인스턴스화합니다.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

7z 아카이브 내에서 PPMd 압축 방법에 대한 설정을 인스턴스화합니다.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| maxOrder | Byte | 최대 주문. |
| suballocatorSize | Int32 | MB 하위 할당자의 메모리 크기가 소모될 수 있습니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* 2에서 32 사이가 아니거나*suballocatorSize* 1에서 1024 사이가 아닙니다. |

### 비고

더 큰 모델 주문은 거의 확실하게 더 나은 압축과 더 많은 메모리 및 CPU 사용량을 초래합니다.

PPMd 알고리즘은 특히 큰 파일에 사용하거나 큰 모델 순서와 함께 사용할 때 많은 메모리가 필요할 수 있습니다.

### 예

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 또한보십시오

* class [SevenZipPPMdCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

기본 모델 순서 및 하위 할당자 크기로 7z 아카이브 내에서 PPMd 압축 방법에 대한 설정을 인스턴스화합니다.

```csharp
public SevenZipPPMdCompressionSettings()
```

### 비고

기본 모델 순서는 6이고 하위 할당자 크기는 16MB입니다.

### 예

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 또한보십시오

* class [SevenZipPPMdCompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* 집회 [Aspose.Zip](../../../)


