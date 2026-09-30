---
title: "클래스 AppleArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Apple.AppleArchive 클래스. 이 클래스는 Apple Archive .aar 파일을 나타냅니다. Apple Archive 파일을 구성하는 데 사용하십시오."
type: docs
weight: 60
url: /ko/net/aspose.zip.apple/applearchive/
---
## AppleArchive class

이 클래스는 Apple Archive (.aar) 파일을 나타냅니다. 이를 사용하여 Apple Archive 파일을 구성할 수 있습니다.

```csharp
public class AppleArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [AppleArchive](applearchive/#constructor)(AppleArchiveEntrySettings) | `AppleArchive` 클래스의 새 인스턴스를 초기화하고, 구성된 항목에 사용되는 설정을 적용합니다. |
| [AppleArchive](applearchive/#constructor_1)(Stream, AppleArchiveLoadOptions) | `AppleArchive` 클래스의 새 인스턴스를 초기화하고, 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [AppleArchive](applearchive/#constructor_2)(string, AppleArchiveLoadOptions) | `AppleArchive` 클래스의 새 인스턴스를 초기화하고, 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.apple/applearchive/entries/) { get; } | 아카이브를 구성하는 항목을 가져옵니다. |
| [IsSolid](../../aspose.zip.apple/applearchive/issolid/) { get; } | 아카이브가 솔리드 압축을 사용하는지 여부를 나타내는 값을 가져옵니다. 솔리드 모드에서는 모든 항목 데이터가 단일 스트림으로 압축되며 개별 항목 추출이 불가능합니다. 대신 [`ExtractToDirectory`](../../aspose.zip/iarchive/extracttodirectory/)를 사용하십시오. |
| [NewEntrySettings](../../aspose.zip.apple/applearchive/newentrysettings/) { get; } | 새로 구성된 항목에 사용되는 설정을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CreateEntries](../../aspose.zip.apple/applearchive/createentries/)(DirectoryInfo, bool) | 지정된 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_1)(string, Stream) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry)(string, FileInfo, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.apple/applearchive/createentry/#createentry_2)(string, string, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [Dispose](../../aspose.zip.apple/applearchive/dispose/)() | 관리되지 않는 리소스를 해제, 릴리스 또는 재설정과 관련된 애플리케이션 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip.apple/applearchive/extracttodirectory/)(string) | 아카이브의 모든 파일을 제공된 디렉터리로 추출합니다. |
| [Save](../../aspose.zip.apple/applearchive/save/#save)(Stream) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.apple/applearchive/save/#save_1)(string) | 제공된 대상 파일에 아카이브를 저장합니다. |

## 비고

Apple 및 Apple Archive는 Apple Inc.의 상표입니다.

### 또 보기

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Apple](../../aspose.zip.apple/)
* assembly [Aspose.Zip](../../)


