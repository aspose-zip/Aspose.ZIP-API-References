---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: .NET API 참조용 Aspose.ZIP
description: Bzip2CompressionSettings 건설자. 의 새 인스턴스를 초기화합니다.Bzip2CompressionSettings 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`Bzip2CompressionSettings`](../) 클래스.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | Int32 | 수백 킬로바이트 단위의 블록 크기. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | 블록 크기가 1에서 9 사이가 아닙니다. |

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [Bzip2CompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* 집회 [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

의 새 인스턴스를 초기화합니다.[`Bzip2CompressionSettings`](../) 기본 블록 크기가 있는 클래스는 900킬로바이트입니다.

```csharp
public Bzip2CompressionSettings()
```

### 예

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 또한보십시오

* class [Bzip2CompressionSettings](../)
* 네임스페이스 [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* 집회 [Aspose.Zip](../../../)


