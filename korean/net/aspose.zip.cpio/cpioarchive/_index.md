---
title: Class CpioArchive
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Cpio.CpioArchive 수업. 이 클래스는 cpio 아카이브 파일을 나타냅니다.
type: docs
weight: 160
url: /ko/net/aspose.zip.cpio/cpioarchive/
---
## CpioArchive class

이 클래스는 cpio 아카이브 파일을 나타냅니다.

```csharp
public class CpioArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [CpioArchive](cpioarchive/#constructor)() | 의 새 인스턴스를 초기화합니다.`CpioArchive` 클래스. |
| [CpioArchive](cpioarchive/#constructor_1)(Stream) | 의 새 인스턴스를 초기화합니다.`CpioArchive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |
| [CpioArchive](cpioarchive/#constructor_2)(string) | 의 새 인스턴스를 초기화합니다.`CpioArchive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.cpio/cpioarchive/entries/) { get; } | 항목 가져오기[`CpioEntry`](../cpioentry/) 아카이브를 구성하는 유형. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries)(DirectoryInfo, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntries](../../aspose.zip.cpio/cpioarchive/createentries/#createentries_1)(string, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_1)(string, Stream) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry)(string, FileInfo, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.cpio/cpioarchive/createentry/#createentry_2)(string, string, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry)(CpioEntry) | 항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다. |
| [DeleteEntry](../../aspose.zip.cpio/cpioarchive/deleteentry/#deleteentry_1)(int) | 항목 목록에서 항목을 index. 로 제거합니다. |
| [Dispose](../../aspose.zip.cpio/cpioarchive/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip.cpio/cpioarchive/extracttodirectory/)(string) | 아카이브의 모든 파일을 제공된 디렉토리에 추출합니다. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save)(Stream, CpioFormat) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.cpio/cpioarchive/save/#save_1)(string, CpioFormat) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped)(Stream, CpioFormat) | gzip 압축을 사용하여 아카이브를 스트림에 저장합니다. |
| [SaveGzipped](../../aspose.zip.cpio/cpioarchive/savegzipped/#savegzipped_1)(string, CpioFormat) | gzip 압축을 사용하여 경로별로 아카이브를 파일에 저장합니다. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed)(Stream, CpioFormat, XzArchiveSettings) | xz 압축을 사용하여 아카이브를 스트림에 저장합니다. |
| [SaveXzCompressed](../../aspose.zip.cpio/cpioarchive/savexzcompressed/#savexzcompressed_1)(string, CpioFormat, XzArchiveSettings) | xz 압축을 사용하여 경로별로 아카이브를 경로에 저장합니다. |

### 또한보십시오

* interface [IArchive](../../aspose.zip/iarchive/)
* 네임스페이스 [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* 집회 [Aspose.Zip](../../)


