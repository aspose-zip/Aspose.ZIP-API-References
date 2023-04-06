---
title: Class Archive
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Archive 수업. 이 클래스는 zip 아카이브 파일을 나타냅니다. zip 아카이브를 작성 추출 또는 업데이트하는 데 사용하십시오.
type: docs
weight: 10
url: /ko/net/aspose.zip/archive/
---
## Archive class

이 클래스는 zip 아카이브 파일을 나타냅니다. zip 아카이브를 작성, 추출 또는 업데이트하는 데 사용하십시오.

```csharp
public class Archive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Archive](archive/#constructor)(ArchiveEntrySettings) | 의 새 인스턴스를 초기화합니다.`Archive` 항목에 대한 선택적 설정이 있는 클래스. |
| [Archive](archive/#constructor_1)(Stream, ArchiveLoadOptions, ArchiveEntrySettings) | 의 새 인스턴스를 초기화합니다.`Archive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |
| [Archive](archive/#constructor_2)(string, ArchiveLoadOptions, ArchiveEntrySettings) | 의 새 인스턴스를 초기화합니다.`Archive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip/archive/entries/) { get; } | 항목 가져오기[`ArchiveEntry`](../archiveentry/) 아카이브를 구성하는 유형. |
| [NewEntrySettings](../../aspose.zip/archive/newentrysettings/) { get; } | 새로 추가된 파일에 사용되는 압축 및 암호화 설정[`ArchiveEntry`](../archiveentry/) 항목. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries)(DirectoryInfo, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntries](../../aspose.zip/archive/createentries/#createentries_1)(string, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_1)(string, Stream, ArchiveEntrySettings) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry)(string, FileInfo, bool, ArchiveEntrySettings) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_2)(string, Stream, ArchiveEntrySettings, FileSystemInfo) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip/archive/createentry/#createentry_3)(string, string, bool, ArchiveEntrySettings) | 아카이브 내에 단일 항목을 생성합니다. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry)(ArchiveEntry) | 항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다. |
| [DeleteEntry](../../aspose.zip/archive/deleteentry/#deleteentry_1)(int) | 항목 목록에서 항목을 index. 로 제거합니다. |
| [Dispose](../../aspose.zip/archive/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip/archive/extracttodirectory/)(string) | 아카이브의 모든 파일을 제공된 디렉토리에 추출합니다. |
| [Save](../../aspose.zip/archive/save/#save)(Stream, ArchiveSaveOptions) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip/archive/save/#save_1)(string, ArchiveSaveOptions) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [SaveSplit](../../aspose.zip/archive/savesplit/)(string, SplitArchiveSaveOptions) | 다중 볼륨 아카이브를 제공된 대상 디렉토리에 저장합니다. |

### 또한보십시오

* interface [IArchive](../iarchive/)
* 네임스페이스 [Aspose.Zip](../../aspose.zip/)
* 집회 [Aspose.Zip](../../)


