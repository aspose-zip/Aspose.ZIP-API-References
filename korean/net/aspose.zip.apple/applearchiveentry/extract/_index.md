---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AppleArchiveEntry 메서드. 제공된 경로에 따라 항목을 파일 시스템에 추출합니다"
type: docs
weight: 50
url: /ko/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다.

```csharp
public FileInfo Extract(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidDataException | 항목에 저장된 체크섬 또는 다이제스트가 추출된 데이터와 일치하지 않습니다. |
| InvalidOperationException | 해당 항목은 합성을 위해 준비된 아카이브에 속하거나, 탐색할 수 없는 아카이브 스트림에서 항목 데이터를 열 수 없습니다. |
| NotSupportedException | 해당 항목은 단일 Apple Archive에 속하거나 지원되지 않는 압축 방식을 사용합니다. |
| ObjectDisposedException | 소스 스트림이 해제되었습니다. |
| IOException | I/O 오류가 발생했습니다. |

### 또 보기

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

제공된 스트림으로 항목을 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 대상 | 스트림 | 대상 스트림. 쓰기 가능해야 합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *destination* 은 `null`입니다. |
| ArgumentException | *destination* 은(는) 쓰기를 지원하지 않습니다. |
| InvalidDataException | 항목에 저장된 체크섬 또는 다이제스트가 추출된 데이터와 일치하지 않습니다. |
| InvalidOperationException | 해당 항목은 합성을 위해 준비된 아카이브에 속하거나, 탐색할 수 없는 아카이브 스트림에서 항목 데이터를 열 수 없습니다. |
| NotSupportedException | 해당 항목은 단일 Apple Archive에 속하거나 지원되지 않는 압축 방식을 사용합니다. |
| ObjectDisposedException | 소스 스트림이 해제되었습니다. |
| IOException | I/O 오류가 발생했습니다. |

### 또 보기

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


