---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: .NET API 참조용 Aspose.ZIP
description: Bzip2SaveOptions 건설자. 의 새 인스턴스를 초기화합니다.Bzip2SaveOptions 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`Bzip2SaveOptions`](../) 클래스.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| blockSize | Int32 | 수백 킬로바이트 단위의 블록 크기. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentOutOfRangeException | 블록 크기가 유효한 범위에 있지 않습니다. |

### 예

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### 또한보십시오

* class [Bzip2SaveOptions](../)
* 네임스페이스 [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* 집회 [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

의 새 인스턴스를 초기화합니다.[`Bzip2SaveOptions`](../) 기본 블록 크기가 있는 클래스는 900킬로바이트입니다.

```csharp
public Bzip2SaveOptions()
```

### 예

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### 또한보십시오

* class [Bzip2SaveOptions](../)
* 네임스페이스 [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* 집회 [Aspose.Zip](../../../)


