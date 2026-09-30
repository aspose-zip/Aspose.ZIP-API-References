---
title: "AlzArchive.ExtractToDirectory"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AlzArchive 메서드. 아카이브에 있는 모든 파일과 디렉터리를 지정된 디렉터리로 추출합니다."
type: docs
weight: 40
url: /ko/net/aspose.zip.alz/alzarchive/extracttodirectory/
---
## AlzArchive.ExtractToDirectory method

아카이브에 있는 모든 파일과 디렉터리를 제공된 디렉터리로 추출합니다.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationDirectory | String | 추출된 파일을 배치할 디렉터리 경로. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *destinationDirectory*가 null입니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 두 개 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| SecurityException | 호출자는 기존 디렉터리에 접근할 권한이 없습니다. |
| NotSupportedException | 디렉터리가 존재하지 않거나, 경로에 드라이브 레이블("C:\")의 일부가 아닌 콜론 문자 (:)가 포함된 경우. |
| ArgumentException | *destinationDirectory*가 길이가 0인 문자열이거나, 공백만 포함하거나, 하나 이상의 잘못된 문자를 포함합니다. 잘못된 문자는 System.IO.Path.GetInvalidPathChars 메서드를 사용하여 확인할 수 있습니다. -or- 경로가 콜론 문자 (:)만 앞에 붙어 있거나 포함되어 있습니다. |
| IOException | path에 지정된 디렉터리가 파일입니다. -or- 네트워크 이름을 알 수 없습니다. |
| InvalidDataException | 잘못된 비밀번호가 제공되었습니다. - 또는 - 아카이브가 손상되었습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 객체가 폐기된 경우에 발생합니다. |

## 비고

디렉터리가 존재하지 않으면 생성됩니다.

## 예제

```csharp
using (var archive = new LhaArchive("archive.lzh")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 또 보기

* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


