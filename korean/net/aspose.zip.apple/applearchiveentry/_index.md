---
title: "클래스 AppleArchiveEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Apple.AppleArchiveEntry 클래스. AppleArchive 내부의 파일 시스템 항목을 나타냅니다"
type: docs
weight: 70
url: /ko/net/aspose.zip.apple/applearchiveentry/
---
## AppleArchiveEntry class

[`AppleArchive`](../applearchive/) 내부의 파일 시스템 항목을 나타냅니다.

```csharp
public sealed class AppleArchiveEntry : IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [IsDirectory](../../aspose.zip.apple/applearchiveentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [IsSymbolicLink](../../aspose.zip.apple/applearchiveentry/issymboliclink/) { get; } | 항목이 심볼릭 링크를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [Length](../../aspose.zip.apple/applearchiveentry/length/) { get; } | 항목의 압축 해제된 길이를 바이트 단위로 가져옵니다. |
| [Name](../../aspose.zip.apple/applearchiveentry/name/) { get; } | 아카이브 내부에서 항목의 경로를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract_1)(Stream) | 제공된 스트림으로 항목을 추출합니다. |
| [Extract](../../aspose.zip.apple/applearchiveentry/extract/#extract)(string) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [Open](../../aspose.zip.apple/applearchiveentry/open/)() | 추출을 위해 항목을 열고 항목 내용이 포함된 스트림을 제공합니다. |

## 비고

이 클래스의 인스턴스는 기존 Apple Archive에서 파싱된 일반 파일, 디렉터리 또는 심볼릭 링크를 나타내거나, 구성 중인 아카이브에 추가된 파일이나 디렉터리를 나타낼 수 있습니다.

### 또 보기

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


