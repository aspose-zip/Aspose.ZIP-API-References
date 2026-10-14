---
title: "EggArchive.EggArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "EggArchive 생성자. 스트림에서 EggArchive 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.zip.egg/eggarchive/eggarchive/
---
## EggArchive(Stream, EggArchiveLoadOptions) {#constructor}

스트림에서 [`EggArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public EggArchive(Stream stream, EggArchiveLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | EGG 아카이브 스트림. 스트림은 읽기 및 탐색을 지원해야 합니다. |
| loadOptions | EggArchiveLoadOptions | 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *stream*이 null입니다. |
| ArgumentException | *stream*은 읽을 수 없으며 탐색할 수 없습니다. |

### 또 보기

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)

---

## EggArchive(string, EggArchiveLoadOptions) {#constructor_1}

파일 경로에서 [`EggArchive`](../) 클래스를 새 인스턴스로 초기화합니다.

```csharp
public EggArchive(string path, EggArchiveLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | EGG 아카이브 파일의 경로. |
| loadOptions | EggArchiveLoadOptions | 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| FileNotFoundException | 파일이 존재하지 않습니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |

### 또 보기

* class [EggArchiveLoadOptions](../../eggarchiveloadoptions/)
* class [EggArchive](../)
* namespace [Aspose.Zip.Egg](../../eggarchive/)
* assembly [Aspose.Zip](../../../)


