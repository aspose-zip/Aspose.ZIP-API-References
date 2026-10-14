---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoArchive 메서드. ISO 이미지에 디렉터리를 추가합니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

ISO 이미지에 디렉터리를 추가합니다.

```csharp
public IsoEntry CreateDirectory(string name)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | ISO 내 디렉터리 경로입니다. |

### 반환 값

ISO 항목이 구성되었습니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브가 추출을 위해 열려 있습니다. |
| ArgumentNullException | `name`은 null이거나 비어 있습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

### 또 보기

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


