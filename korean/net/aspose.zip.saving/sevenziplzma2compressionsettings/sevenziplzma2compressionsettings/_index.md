---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipLZMA2CompressionSettings 건설자. 7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| dictionarySize | Int32 | 히스토리 버퍼의 크기는 4096에서 1073741824 사이여야 합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* 너무 크거나 작습니다. |

### 비고

일반적으로 사전이 클수록 압축률이 좋지만 압축되지 않은 데이터보다 큰 사전은 RAM 낭비입니다.

### 또한보십시오

* class [SevenZipLZMA2CompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

7z 아카이브 내에서 LZMA2 압축 방법에 대한 설정을 인스턴스화합니다.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| dictionarySize | Int32 | 히스토리 버퍼의 크기는 4096에서 1073741824 사이여야 합니다. |
| fastBytes | Int32 | LZMA2 압축기에서 사용하는 빠른 바이트 수를 제어합니다. 더 많은 수의 빠른 바이트는 압축 속도를 희생시키면서 더 나은 압축률을 제공할 수 있습니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* 너무 크거나 너무 작거나,*fastBytes* 너무 크거나 작습니다. |

### 비고

일반적으로 사전이 클수록 압축률이 좋지만 압축되지 않은 데이터보다 큰 사전은 RAM 낭비입니다.

### 또한보십시오

* class [SevenZipLZMA2CompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* 집회 [Aspose.Zip](../../../)


