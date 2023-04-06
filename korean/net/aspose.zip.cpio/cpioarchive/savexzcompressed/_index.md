---
title: CpioArchive.SaveXzCompressed
second_title: .NET API 참조용 Aspose.ZIP
description: CpioArchive 방법. xz 압축을 사용하여 아카이브를 스트림에 저장합니다.
type: docs
weight: 100
url: /ko/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

xz 압축을 사용하여 아카이브를 스트림에 저장합니다.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| output | Stream | 대상 스트림. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |
| settings | XzArchiveSettings | 특정 xz 아카이브 설정 세트: 사전 크기, 블록 크기, 검사 유형. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *output* null입니다. |
| ArgumentException | *output* 쓸 수 없습니다. |

### 비고

*output*스트림은 쓰기 가능해야 합니다.

### 예

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### 또한보십시오

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

xz 압축을 사용하여 경로별로 아카이브를 경로에 저장합니다.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |
| settings | XzArchiveSettings | 특정 xz 아카이브 설정 세트: 사전 크기, 블록 크기, 검사 유형. |

### 예

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### 또한보십시오

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)


