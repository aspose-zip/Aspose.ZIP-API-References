---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarArchive 메서드. 지정된 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

지정된 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceDirectory | String | 압축할 디렉터리입니다. |
| compressionSettings | Boolean | 추가된 [`XarEntry`](../../xarentry/) 항목에 사용되는 압축 설정. |
| includeRootDirectory | XarCompressionSettings | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

Xar 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *sourceDirectory*가 null입니다. |
| SecurityException | 호출자는 *sourceDirectory*에 접근하기 위한 필요한 권한이 없습니다. |
| ArgumentException | *sourceDirectory*에 \", &lt;, &gt;, 또는 &#x7C;와 같은 잘못된 문자가 포함되어 있습니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 두 개 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고, 파일 이름은 260자 미만이어야 합니다. 지정된 경로, 파일 이름 또는 두 개 모두가 너무 깁니다. |
| IOException | *sourceDirectory*는 디렉터리가 아니라 파일을 나타냅니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### 또 보기

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

지정된 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| directory | DirectoryInfo | 압축할 디렉터리입니다. |
| compressionSettings | Boolean | 추가된 [`XarEntry`](../../xarentry/) 항목에 사용되는 압축 설정. |
| includeRootDirectory | XarCompressionSettings | 루트 디렉터리 자체를 포함할지 여부를 나타냅니다. |

### 반환 값

Xar 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *directory*이 null입니다. |
| SecurityException | 호출자가 *directory*에 접근할 권한이 없습니다. |
| IOException | *directory*는 디렉터리가 아니라 파일을 나타냅니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### 또 보기

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


