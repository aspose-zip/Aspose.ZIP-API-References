---
title: Archive.SaveSplit
second_title: .NET API 참조용 Aspose.ZIP
description: Archive 방법. 다중 볼륨 아카이브를 제공된 대상 디렉토리에 저장합니다.
type: docs
weight: 100
url: /ko/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

다중 볼륨 아카이브를 제공된 대상 디렉토리에 저장합니다.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | String | 아카이브 세그먼트를 생성할 디렉토리 경로. |
| options | SplitArchiveSaveOptions | 파일 이름을 포함한 아카이브 저장 옵션. |

### 예외

| 예외 | 상태 |
| --- | --- |
| InvalidOperationException | 이 아카이브는 기존 소스에서 열렸습니다. |
| NotSupportedException | 이 아카이브는 XZ 방식으로 압축되고 암호화됩니다. |
| ArgumentNullException | *destinationDirectory* null입니다. |
| SecurityException | 호출자에게 디렉토리에 액세스하는 데 필요한 권한이 없습니다. |
| ArgumentException | *destinationDirectory* ", &gt;, &lt; 또는 &#x7C;와 같은 유효하지 않은 문자가 포함되어 있습니다. |
| PathTooLongException | 지정된 경로가 시스템 정의 최대 길이를 초과합니다. |

### 비고

이 방법은 여러 가지(`N`) 파일 filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

기존 아카이브를 다중 볼륨으로 만들 수 없습니다.

### 예

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### 또한보십시오

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)


