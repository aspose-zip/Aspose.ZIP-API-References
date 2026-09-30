---
title: "GetFormatInfo"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: 
type: docs
weight: 20
url: /ko/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

형식 정보를 가져옵니다.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileName | String | 아카이브 파일의 파일 이름입니다. |

### 반환 값

아카이브 형식에 대한 정보이며, 형식이 감지되지 않은 경우 null입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *fileName*은 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *fileName*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *fileName* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *fileName*이 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로 길이가 248자 미만이어야 하고, 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *fileName* 위치의 파일 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| IOException | 파일을 여는 중 I/O 오류가 발생했습니다. |

### 또 보기

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

형식 정보를 가져옵니다.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | 아카이브 파일의 스트림입니다. |

### 반환 값

아카이브 형식에 대한 정보이며, 형식이 감지되지 않은 경우 null입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *stream*이 null입니다. |
| ArgumentException | *stream*은(는) 탐색이 불가능합니다. |

### 또 보기

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- 편집 금지: xmldocmd에 의해 Aspose.Zip.dll용으로 생성되었습니다 -->
