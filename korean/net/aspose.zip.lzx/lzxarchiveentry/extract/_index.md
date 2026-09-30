---
title: "LzxArchiveEntry.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "LzxArchiveEntry 메서드. Lzx 아카이브 항목을 경로에 따라 파일 시스템에 추출합니다"
type: docs
weight: 80
url: /ko/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

경로를 통해 Lzx 아카이브 항목을 파일 시스템에 추출합니다.

```csharp
public FileSystemInfo Extract(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 압축 해제된 데이터를 저장할 파일 경로. |

### 반환 값

추출된 데이터를 포함하는 FileSystemInfoInstance.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브 헤더와 서비스 정보가 읽히지 않았습니다. |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| InvalidDataException | 헤더 또는 데이터의 체크섬이 일치하지 않습니다. - 또는 - 아카이브가 손상되었습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| NotSupportedException | 잘못된 압축 방식입니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| EndOfStreamException | 스트림의 끝에 예기치 않게 도달했을 때 발생합니다. |

## 예제

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### 또 보기

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

제공된 스트림으로 항목을 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 대상 | 스트림 | 대상 스트림. 쓰기 가능해야 합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | *destination* 은(는) 쓰기를 지원하지 않습니다. |
| InvalidDataException | 헤더 또는 데이터의 체크섬이 일치하지 않습니다. - 또는 - 아카이브가 손상되었습니다. |
| ArgumentNullException | 대상 스트림이 null입니다. |
| NotSupportedException | 잘못된 압축 방식입니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| EndOfStreamException | 스트림의 끝에 예기치 않게 도달했을 때 발생합니다. |

### 또 보기

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


