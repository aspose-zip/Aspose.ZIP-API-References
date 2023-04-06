---
title: Class SevenZipArchive
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.SevenZip.SevenZipArchive 수업. 이 클래스는 7z 아카이브 파일을 나타냅니다. 7z 아카이브를 구성하고 추출하는 데 사용하십시오.
type: docs
weight: 660
url: /ko/net/aspose.zip.sevenzip/sevenziparchive/
---
## SevenZipArchive class

이 클래스는 7z 아카이브 파일을 나타냅니다. 7z 아카이브를 구성하고 추출하는 데 사용하십시오.

```csharp
public class SevenZipArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [SevenZipArchive](sevenziparchive/#constructor)(SevenZipEntrySettings) | 의 새 인스턴스를 초기화합니다.`SevenZipArchive` 항목에 대한 선택적 설정이 있는 클래스. |
| [SevenZipArchive](sevenziparchive/#constructor_1)(Stream) | 의 새 인스턴스를 초기화합니다.`SevenZipArchive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |
| [SevenZipArchive](sevenziparchive/#constructor_2)(string) | 의 새 인스턴스를 초기화합니다.`SevenZipArchive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.sevenzip/sevenziparchive/entries/) { get; } | 항목 가져오기[`SevenZipArchiveEntry`](../sevenziparchiveentry/) 아카이브를 구성하는 유형. |
| [NewEntrySettings](../../aspose.zip.sevenzip/sevenziparchive/newentrysettings/) { get; } | 새로 추가된 파일에 사용되는 압축 및 암호화 설정[`SevenZipArchiveEntry`](../sevenziparchiveentry/) 항목. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries)(DirectoryInfo, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntries](../../aspose.zip.sevenzip/sevenziparchive/createentries/#createentries_1)(string, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_1)(string, Stream, SevenZipEntrySettings) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry)(string, FileInfo, bool, SevenZipEntrySettings) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_2)(string, Stream, SevenZipEntrySettings, FileSystemInfo) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.sevenzip/sevenziparchive/createentry/#createentry_3)(string, string, bool, SevenZipEntrySettings) | 아카이브 내에 단일 항목을 생성합니다. |
| [Dispose](../../aspose.zip.sevenzip/sevenziparchive/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip.sevenzip/sevenziparchive/extracttodirectory/)(string, string) | 아카이브의 모든 파일을 제공된 디렉토리에 추출합니다. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save)(Stream) | 제공된 스트림에 7z 아카이브를 저장합니다. |
| [Save](../../aspose.zip.sevenzip/sevenziparchive/save/#save_1)(string) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [SaveSplit](../../aspose.zip.sevenzip/sevenziparchive/savesplit/)(string, SplitSevenZipArchiveSaveOptions) | 다중 볼륨 아카이브를 제공된 대상 디렉토리에 저장합니다. |

### 또한보십시오

* interface [IArchive](../../aspose.zip/iarchive/)
* 네임스페이스 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* 집회 [Aspose.Zip](../../)


