---
title: "AppleArchiveEntry.Open"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AppleArchiveEntry 메서드. 항목을 추출하기 위해 열고 항목 내용을 포함하는 스트림을 제공합니다"
type: docs
weight: 60
url: /ko/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

추출을 위해 항목을 열고 항목 내용이 포함된 스트림을 제공합니다.

```csharp
public Stream Open()
```

### 반환 값

추출된 항목 데이터를 포함하는 읽기 가능한 스트림입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| NotSupportedException | 해당 항목은 단일 Apple Archive에 속하거나 지원되지 않는 압축 방식을 사용합니다. |
| InvalidDataException | 항목에 저장된 체크섬 또는 다이제스트가 추출된 데이터와 일치하지 않습니다. |
| InvalidOperationException | 해당 항목은 합성을 위해 준비된 아카이브에 속하거나, 탐색할 수 없는 아카이브 스트림에서 항목 데이터를 열 수 없습니다. |
| ObjectDisposedException | 소스 스트림이 해제되었습니다. |
| IOException | I/O 오류가 발생했습니다. |

## 비고

반환된 스트림을 읽어 원본 항목 내용을 가져옵니다. 아카이브에 체크섬 필드가 포함된 경우, 반환된 스트림을 읽는 동안 체크섬이 검증됩니다.

### 또 보기

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


