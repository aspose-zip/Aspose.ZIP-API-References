---
title: "IsoArchive.ExtractToDirectory"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoArchive 메서드. 지정된 디렉터리로 모든 항목을 추출합니다"
type: docs
weight: 60
url: /ko/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

지정된 디렉터리로 모든 항목을 추출합니다.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationDirectory | String | 항목을 추출할 디렉터리입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브가 편집 모드에 있을 때 발생합니다. |
| ArgumentNullException | *destinationDirectory*가 null일 때 발생합니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다:

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 또 보기

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


