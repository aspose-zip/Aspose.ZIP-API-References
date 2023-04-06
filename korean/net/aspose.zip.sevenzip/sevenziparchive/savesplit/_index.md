---
title: SevenZipArchive.SaveSplit
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipArchive 방법. 다중 볼륨 아카이브를 제공된 대상 디렉토리에 저장합니다.
type: docs
weight: 90
url: /ko/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

다중 볼륨 아카이브를 제공된 대상 디렉토리에 저장합니다.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | String | 아카이브 세그먼트를 생성할 디렉토리 경로. |
| options | SplitSevenZipArchiveSaveOptions | 파일 이름을 포함한 아카이브 저장 옵션. |

### 예외

| 예외 | 상태 |
| --- | --- |
| InvalidOperationException | 이 아카이브는 기존 소스에서 열렸습니다. |
| ArgumentNullException | *destinationDirectory* null입니다. |
| SecurityException | 호출자에게 디렉토리에 액세스하는 데 필요한 권한이 없습니다. |
| ArgumentException | *destinationDirectory* ", &gt;, &lt; 또는 &#x7C;와 같은 유효하지 않은 문자가 포함되어 있습니다. |
| PathTooLongException | 지정된 경로가 시스템 정의 최대 길이를 초과합니다. |

### 비고

이 방법은 여러 가지(`N`) 파일 filename.7z.001, filename.7z.002, ..., filename.7z.(n).

기존 아카이브를 다중 볼륨으로 만들 수 없습니다.

### 예

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### 또한보십시오

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)


