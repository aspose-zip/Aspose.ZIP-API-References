---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: .NET API 참조용 Aspose.ZIP
description: ArchiveInstanceInfo 방법. 아카이브 인스턴스 정보를 가져옵니다.
type: docs
weight: 10
url: /ko/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

아카이브 인스턴스 정보를 가져옵니다.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileName | String | 아카이브 파일의 파일 이름입니다. |

### 반환 값

아카이브 인스턴스에 대한 정보 또는 형식이 감지되지 않은 경우 null입니다.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *fileName* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*fileName* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*fileName* 거부되었습니다. |
| PathTooLongException | 지정된*fileName* 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*fileName* 문자열 중간에 콜론(:)을 포함합니다. |
| IOException | 파일을 여는 동안 I/O 오류가 발생했습니다. |

### 또한보십시오

* class [ArchiveInstanceInfo](../)
* 네임스페이스 [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* 집회 [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

아카이브 인스턴스 정보를 가져옵니다.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| stream | Stream | 아카이브 파일의 스트림입니다. |

### 반환 값

아카이브 인스턴스에 대한 정보 또는 형식이 감지되지 않은 경우 null입니다.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *stream* null입니다. |
| ArgumentException | *stream* 찾을 수 없습니다. |

### 또한보십시오

* class [ArchiveInstanceInfo](../)
* 네임스페이스 [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* 집회 [Aspose.Zip](../../../)


