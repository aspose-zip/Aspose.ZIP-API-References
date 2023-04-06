---
title: XzArchiveSettings.XzArchiveSettings
second_title: .NET API 참조용 Aspose.ZIP
description: XzArchiveSettings 건설자. 의 새 인스턴스를 초기화합니다.XzArchiveSettings 단일 LZMA2 압축을 사용하는 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

의 새 인스턴스를 초기화합니다.[`XzArchiveSettings`](../) 단일 LZMA2 압축을 사용하는 클래스.

```csharp
public XzArchiveSettings()
```

### 비고

LZMA2 필터의 기본 사전 크기는 16MB, 기본 블록 크기는 64MB, 기본 체크섬 유형은 CRC32입니다.

### 또한보십시오

* class [XzArchiveSettings](../)
* 네임스페이스 [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* 집회 [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`XzArchiveSettings`](../) 맞춤 매개변수가 있는 클래스.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| filters | XzFilterSettings[] | 필터(압축기)를 순차적으로 적용하여 생성[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . 그것은 하나 일 수 있습니다[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) 또는 쌍[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) 그리고[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | 크기 xz 아카이브 블록. |
| checkType | XzCheckType | 압축되지 않은 데이터에 대한 체크섬 계산 유형입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* 음수입니다. |
| ArgumentNullException | *filters* null입니다 |
| ArgumentException | *filters* 1개 미만 또는 2개 이상의 필터가 있거나 마지막 필터가[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### 예

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### 또한보십시오

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* 네임스페이스 [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* 집회 [Aspose.Zip](../../../)


