---
title: RarArchive.ExtractToDirectory
second_title: .NET API 참조용 Aspose.ZIP
description: RarArchive 방법. 아카이브의 모든 파일을 제공된 디렉토리에 추출합니다.
type: docs
weight: 40
url: /ko/net/aspose.zip.rar/rararchive/extracttodirectory/
---
## RarArchive.ExtractToDirectory method

아카이브의 모든 파일을 제공된 디렉토리에 추출합니다.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | String | 압축을 푼 파일을 저장할 디렉토리의 경로입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *destinationDirectory* null입니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| SecurityException | 호출자에게 기존 디렉터리에 액세스하는 데 필요한 권한이 없습니다. |
| NotSupportedException | 디렉토리가 존재하지 않는 경우 경로에는 드라이브 레이블("C:\")의 일부가 아닌 콜론 문자(:)가 포함됩니다. |
| ArgumentException | *destinationDirectory* 길이가 0인 문자열이거나 공백만 포함하거나 하나 이상의 잘못된 문자를 포함합니다. System.IO.Path.GetInvalidPathChars 메서드를 사용하여 잘못된 문자를 쿼리할 수 있습니다. -또는- 경로에 콜론 문자(:)만 붙거나 포함합니다. |
| IOException | 경로로 지정된 디렉토리는 파일입니다. - 또는 - 네트워크 이름을 알 수 없습니다. |

### 비고

디렉토리가 존재하지 않으면 생성됩니다.

### 예

```csharp
using (var archive = new RarArchive("archive.rar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 또한보십시오

* class [RarArchive](../)
* 네임스페이스 [Aspose.Zip.Rar](../../rararchive/)
* 집회 [Aspose.Zip](../../../)


