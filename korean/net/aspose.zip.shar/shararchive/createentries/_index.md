---
title: SharArchive.CreateEntries
second_title: .NET API 참조용 Aspose.ZIP
description: SharArchive 방법. 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.
type: docs
weight: 30
url: /ko/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceDirectory | String | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

Shar 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *sourceDirectory* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다.*sourceDirectory*. |
| ArgumentException | *sourceDirectory* ", &lt;, &gt; 또는 &#x7C;와 같은 유효하지 않은 문자가 포함되어 있습니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. 지정된 경로, 파일 이름 또는 둘 다 너무 깁니다. |
| IOException | *sourceDirectory* 디렉토리가 아니라 파일을 나타냅니다. |

### 예

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### 또한보십시오

* class [SharArchive](../)
* 네임스페이스 [Aspose.Zip.Shar](../../shararchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| directory | DirectoryInfo | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

Shar 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *directory* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다.*directory*. |
| IOException | *directory* 디렉토리가 아니라 파일을 나타냅니다. |

### 예

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### 또한보십시오

* class [SharArchive](../)
* 네임스페이스 [Aspose.Zip.Shar](../../shararchive/)
* 집회 [Aspose.Zip](../../../)


