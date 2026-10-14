---
title: "IsoEntry.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoEntry 메서드. 제공된 경로에 따라 항목을 파일 시스템에 추출합니다"
type: docs
weight: 50
url: /ko/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다.

```csharp
public FileInfo Extract(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

### 반환 값

추출된 데이터를 포함하는 FileInfo 인스턴스.

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
| InvalidOperationException | 아카이브 헤더와 서비스 정보가 읽히지 않았습니다. |

### 또 보기

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
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
| NotSupportedException | 항목이 파일을 나타내지 않을 경우 예외를 발생시킵니다. |
| ArgumentException | 제공된 스트림이 쓰기를 지원하지 않습니다. |

### 또 보기

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


