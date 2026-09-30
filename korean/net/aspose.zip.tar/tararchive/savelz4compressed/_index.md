---
title: "TarArchive.SaveLZ4Compressed"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "TarArchive 메서드. LZ4 압축을 사용하여 스트림에 아카이브를 저장합니다"
type: docs
weight: 170
url: /ko/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

LZ4 압축을 사용하여 스트림에 아카이브를 저장합니다.

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| output | 스트림 | 대상 스트림. |
| 형식 | Nullable`1 | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *output*이 null입니다. |
| ArgumentException | *output*은(는) 쓰기 가능하지 않습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| IOException | I/O 오류가 발생했습니다. |

## 비고

*output* must be writable.

## 예제

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### 또 보기

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

LZ4 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다.

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |
| 형식 | Nullable`1 | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| UnauthorizedAccessException | 호출자에게 필요한 권한이 없습니다. -or- *path*가 읽기 전용 파일 또는 디렉터리를 지정했습니다. |
| ArgumentException | *path*가 길이가 0인 문자열이거나, 공백만 포함하거나, InvalidPathChars에 정의된 하나 이상의 잘못된 문자를 포함하고 있습니다. |
| ArgumentNullException | *path*이 null입니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| DirectoryNotFoundException | 지정된 *path*가 유효하지 않습니다(예: 매핑되지 않은 드라이브에 있습니다). |
| NotSupportedException | *path*가 잘못된 형식입니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| IOException | I/O 오류가 발생했습니다. |

## 예제

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### 또 보기

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


