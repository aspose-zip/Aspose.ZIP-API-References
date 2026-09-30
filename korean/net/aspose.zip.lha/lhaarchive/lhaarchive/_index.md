---
title: "LhaArchive.LhaArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "LhaArchive 생성자. LhaArchive 클래스를 새 인스턴스로 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다."
type: docs
weight: 10
url: /ko/net/aspose.zip.lha/lhaarchive/lhaarchive/
---
## LhaArchive(Stream, LhaLoadOptions) {#constructor}

새 인스턴스의 [`LhaArchive`](../) 클래스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

```csharp
public LhaArchive(Stream sourceStream, LhaLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceStream | 스트림 | 아카이브의 소스입니다. |
| loadOptions | LhaLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *sourceStream*이 null입니다. |
| ArgumentException | *sourceStream*은(는) 탐색할 수 없습니다. |
| InvalidDataException | 부적절한 데이터가 발견되었습니다. |
| EndOfStreamException | 예상된 바이트 수가 읽히기 전에 스트림의 끝에 도달하면 발생합니다. |
| ObjectDisposedException | 객체가 폐기된 경우에 발생합니다. |

## 비고

이 생성자는 어떤 항목도 압축을 해제하지 않습니다. 압축 해제를 위해 [`Extract`](../../lhaarchiveentry/extract/) 메서드를 참조하십시오.

### 또 보기

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)

---

## LhaArchive(string, LhaLoadOptions) {#constructor_1}

새 인스턴스의 [`LhaArchive`](../) 클래스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

```csharp
public LhaArchive(string path, LhaLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일에 대한 전체 경로나 상대 경로입니다. |
| loadOptions | LhaLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |
| InvalidDataException | 파일이 손상되었습니다. |
| EndOfStreamException | 예상된 바이트 수가 읽히기 전에 스트림의 끝에 도달하면 발생합니다. |
| ObjectDisposedException | 객체가 폐기된 경우에 발생합니다. |

## 비고

이 생성자는 어떤 항목도 압축을 해제하지 않습니다. 압축 해제를 위해 [`Extract`](../../lhaarchiveentry/extract/) 메서드를 참조하십시오.

## 예제

다음 예제는 아카이브를 추출한 다음 첫 번째 항목을 `MemoryStream`으로 압축 해제합니다.

```csharp
var extracted = new MemoryStream();
using (LhaArchive archive = new LhaArchive("sample.lzh"))
{
    archive.Entries[0].Extract(extracted);
}
```

### 또 보기

* class [LhaLoadOptions](../../lhaloadoptions/)
* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


