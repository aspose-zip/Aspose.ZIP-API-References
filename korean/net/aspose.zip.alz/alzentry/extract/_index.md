---
title: "AlzEntry.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AlzEntry 메서드. 제공된 경로에 따라 항목을 파일 시스템에 추출합니다."
type: docs
weight: 60
url: /ko/net/aspose.zip.alz/alzentry/extract/
---
## Extract(string, string) {#extract}

제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다.

```csharp
public FileInfo Extract(string path, string password = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |
| 비밀번호 | String | 복호화를 위한 선택적 비밀번호. |

### 반환 값

조합된 파일의 파일 정보입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| InvalidDataException | 아카이브가 손상되었습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |

## 예제

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### 또 보기

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream, string) {#extract_1}

제공된 스트림으로 항목을 추출합니다.

```csharp
public void Extract(Stream destination, string password = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 대상 | 스트림 | 대상 스트림. 쓰기 가능해야 합니다. |
| 비밀번호 | String | 복호화를 위한 선택적 비밀번호. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | *destination* 은(는) 쓰기를 지원하지 않습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 열려 있지 않습니다. - 또는 - 이 항목은 디렉터리입니다. |
| InvalidDataException | 항목 내에 잘못된 데이터가 있습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |

## 예제

비밀번호를 사용하여 ALZ 아카이브의 항목을 추출합니다.

```csharp
using (var archive = new SevenZipArchive("archive.7z"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### 또 보기

* class [AlzEntry](../)
* namespace [Aspose.Zip.Alz](../../alzentry/)
* assembly [Aspose.Zip](../../../)


