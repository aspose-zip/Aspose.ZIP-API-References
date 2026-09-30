---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "CpioArchive 메서드. Z 압축으로 스트림에 아카이브를 저장합니다."
type: docs
weight: 130
url: /ko/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Z 압축으로 스트림에 아카이브를 저장합니다.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| output | 스트림 | 대상 스트림. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *output*이 null입니다. |
| ArgumentException | *output*은(는) 쓰기 가능하지 않습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

*output* must be writable.

## 예제

```csharp
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
        }
    }
}
```

### 또 보기

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Z 압축으로 경로에 아카이브를 저장합니다.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| ArgumentNullException | *path*는 `null`입니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다(예: 매핑되지 않은 드라이브에 있는 경우). |
| IOException | I/O 오류가 발생했습니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 둘 다가 시스템에서 정의한 최대 길이를 초과합니다. |

## 예제

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### 또 보기

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


