---
title: CpioArchive.SaveGzipped
second_title: .NET API 참조용 Aspose.ZIP
description: CpioArchive 방법. gzip 압축을 사용하여 아카이브를 스트림에 저장합니다.
type: docs
weight: 90
url: /ko/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

gzip 압축을 사용하여 아카이브를 스트림에 저장합니다.

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| output | Stream | 대상 스트림. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *output* null입니다. |
| ArgumentException | *output* 쓸 수 없습니다. |

### 비고

*output*쓰기 가능해야 합니다.

### 예

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### 또한보십시오

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

gzip 압축을 사용하여 경로별로 아카이브를 파일에 저장합니다.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |

### 예

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### 또한보십시오

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)


