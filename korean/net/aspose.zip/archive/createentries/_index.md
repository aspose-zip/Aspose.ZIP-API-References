---
title: Archive.CreateEntries
second_title: .NET API 참조용 Aspose.ZIP
description: Archive 방법. 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.
type: docs
weight: 40
url: /ko/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| directory | DirectoryInfo | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

항목이 구성된 아카이브.

### 예외

| 예외 | 상태 |
| --- | --- |
| DirectoryNotFoundException | 가는 길*directory* 매핑되지 않은 드라이브에 있는 것과 같이 유효하지 않습니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다.*directory*. |

### 예

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### 또한보십시오

* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceDirectory | String | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

항목이 구성된 아카이브.

### 예

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### 또한보십시오

* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)


