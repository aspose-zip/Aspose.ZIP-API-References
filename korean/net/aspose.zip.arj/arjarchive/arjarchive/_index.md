---
title: "ArjArchive.ArjArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ArjArchive 생성자. ArjArchive 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다."
type: docs
weight: 10
url: /ko/net/aspose.zip.arj/arjarchive/arjarchive/
---
## ArjArchive(Stream, ArjLoadOptions) {#constructor}

[`ArjArchive`](../) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

```csharp
public ArjArchive(Stream extractionSource, ArjLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| extractionSource | 스트림 | 아카이브의 소스입니다. |
| loadOptions | ArjLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *extractionSource* 가 null 입니다. |
| ArgumentException | &gt;*extractionSource* 은(는) 검색을 지원하지 않습니다. |
| InvalidDataException | 아카이브 서명이 잘못되었습니다. - 또는 - 파일이 ARJ 아카이브가 아닙니다. |
| EndOfStreamException | 스트림의 끝에 도달했지만 모든 헤더 바이트 또는 이름 바이트가 읽히기 전에 발생합니다. |
| NotSupportedException | 아카이브가 손상되었습니다. |

## 비고

이 생성자는 어떤 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [`Extract`](../../arjentryplain/extract/) 메서드를 참조하세요.

### 또 보기

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)

---

## ArjArchive(string, ArjLoadOptions) {#constructor_1}

[`ArjArchive`](../) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

```csharp
public ArjArchive(string path, ArjLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일의 경로입니다. |
| loadOptions | ArjLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

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
| EndOfStreamException | 스트림의 끝에 도달했지만 모든 헤더 바이트 또는 이름 바이트가 읽히기 전에 발생합니다. |
| InvalidDataException | ARJ 매직 번호가 유효하지 않거나 헤더 크기가 범위를 벗어났습니다. |

## 비고

이 생성자는 어떤 항목도 풀지 않습니다. 압축 해제를 위해 [`Extract`](../../arjentryplain/extract/) 메서드를 참조하세요.

## 예제

다음 예제에서는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```csharp
using (var archive = new ArjArchive("archive.arj")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 또 보기

* class [ArjLoadOptions](../../arjloadoptions/)
* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


