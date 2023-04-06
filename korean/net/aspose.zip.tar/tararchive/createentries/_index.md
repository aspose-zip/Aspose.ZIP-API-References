---
title: TarArchive.CreateEntries
second_title: .NET API 참조용 Aspose.ZIP
description: TarArchive 방법. 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.
type: docs
weight: 70
url: /ko/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| directory | DirectoryInfo | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

항목이 구성된 아카이브.

### 예

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### 또한보십시오

* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceDirectory | String | 압축할 디렉터리입니다. |
| includeRootDirectory | Boolean | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

항목이 구성된 아카이브.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *sourceDirectory* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다.*sourceDirectory*. |
| ArgumentException | *sourceDirectory* ", &lt;, &gt; 또는 &#x7C;와 같은 유효하지 않은 문자가 포함되어 있습니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. 지정된 경로, 파일 이름 또는 둘 다 너무 깁니다. |

### 예

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### 또한보십시오

* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)


