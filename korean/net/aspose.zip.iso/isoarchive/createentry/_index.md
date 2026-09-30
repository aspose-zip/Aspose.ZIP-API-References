---
title: "IsoArchive.CreateEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoArchive 메서드. 파일을 ISO 이미지에 추가합니다."
type: docs
weight: 40
url: /ko/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

ISO 이미지에 파일을 추가합니다.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | ISO 내 파일의 경로. |
| filePath | String | 파일의 경로. |

### 반환 값

ISO 항목이 구성되었습니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *filePath*이 null입니다. |
| ArgumentException | *filePath*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *filePath* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *filePath*이 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *filePath* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| IOException | 파일을 여는 중 I/O 오류가 발생했습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다(예: 매핑되지 않은 드라이브에 있는 경우). |
| FileNotFoundException | *filePath*에 지정된 파일을 찾을 수 없습니다. |
| InvalidOperationException | 아카이브가 편집 모드가 아닙니다. |

### 또 보기

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

ISO 이미지에 파일을 추가합니다.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | ISO 내 파일의 경로. |
| 소스 | 스트림 | 파일 데이터를 포함하는 스트림. |

### 반환 값

ISO 항목이 구성되었습니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| ArgumentNullException | *name* 또는 *source*가 null인 경우 발생합니다. |
| InvalidOperationException | 아카이브가 편집 모드가 아닙니다. |

### 또 보기

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

ISO 이미지에 파일을 추가합니다.

```csharp
public IsoEntry CreateEntry(string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | ISO 내 디렉터리 경로입니다. |

### 반환 값

ISO 항목이 구성되었습니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | `name`은 null이거나 비어 있습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 열려 있습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

### 또 보기

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


