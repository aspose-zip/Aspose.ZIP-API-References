---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "CabArchive 메서드. 지정된 디렉터리에서 모든 파일을 재귀적으로 아카이브에 추가합니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

지정된 디렉터리에서 모든 파일을 재귀적으로 아카이브에 추가합니다.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| directory | DirectoryInfo | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 항목 경로에 루트 디렉터리 이름을 포함할지 여부를 나타냅니다. |

### 반환 값

현재 [`CabArchive`](../) 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *directory*이 null입니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| DirectoryNotFoundException | *directory*을(를) 찾을 수 없습니다. |
| SecurityException | 호출자는 *directory* 또는 그 내용에 접근할 권한이 없습니다. |
| UnauthorizedAccessException | *directory* 또는 그 파일 중 하나에 대한 접근이 거부되었습니다. |
| IOException | 디렉터리 *directory*에 접근하는 동안 I/O 오류가 발생했습니다. |
| PathTooLongException | 생성된 항목 경로가 시스템에서 정의한 최대 길이를 초과했습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되어 있어 항목을 추가할 수 없습니다. |

## 예제

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### 또 보기

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

지정된 디렉터리 경로에서 모든 파일을 재귀적으로 아카이브에 추가합니다.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceDirectory | String | 압축할 디렉터리 경로. |
| includeRootDirectory | Boolean | 항목 경로에 루트 디렉터리 이름을 포함할지 여부를 나타냅니다. |

### 반환 값

현재 [`CabArchive`](../) 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| ArgumentNullException | *sourceDirectory*가 null입니다. |
| DirectoryNotFoundException | *sourceDirectory*를 찾을 수 없습니다. |
| SecurityException | 호출자는 *sourceDirectory*에 접근하기 위한 필요한 권한이 없습니다. |
| UnauthorizedAccessException | *sourceDirectory*에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *sourceDirectory*가 시스템에서 정의한 최대 길이를 초과했습니다. |
| ArgumentException | *sourceDirectory*가 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| IOException | *sourceDirectory*에 접근하는 동안 I/O 오류가 발생했습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되어 있어 항목을 추가할 수 없습니다. |

## 예제

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### 또 보기

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


