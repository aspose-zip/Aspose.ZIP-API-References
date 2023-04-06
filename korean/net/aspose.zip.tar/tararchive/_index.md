---
title: Class TarArchive
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Tar.TarArchive 수업. 이 클래스는 tar 아카이브 파일을 나타냅니다. tar 아카이브를 작성 추출 또는 업데이트하는 데 사용하십시오.
type: docs
weight: 730
url: /ko/net/aspose.zip.tar/tararchive/
---
## TarArchive class

이 클래스는 tar 아카이브 파일을 나타냅니다. tar 아카이브를 작성, 추출 또는 업데이트하는 데 사용하십시오.

```csharp
public class TarArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TarArchive](tararchive/#constructor)() | 의 새 인스턴스를 초기화합니다.`TarArchive` 클래스. |
| [TarArchive](tararchive/#constructor_1)(Stream) | 의 새 인스턴스를 초기화합니다.[`Archive`](../../aspose.zip/archive/) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |
| [TarArchive](tararchive/#constructor_2)(string) | 의 새 인스턴스를 초기화합니다.`TarArchive` 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.tar/tararchive/entries/) { get; } | 항목 가져오기[`TarEntry`](../tarentry/) 아카이브를 구성하는 유형. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip)(Stream) | 제공된 gzip 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromGZip](../../aspose.zip.tar/tararchive/fromgzip/#fromgzip_1)(string) | 제공된 gzip 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip)(Stream) | 제공된 lzip 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromLZip](../../aspose.zip.tar/tararchive/fromlzip/#fromlzip_1)(string) | 제공된 lzip 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz)(Stream) | 제공된 xz 형식 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromXz](../../aspose.zip.tar/tararchive/fromxz/#fromxz_1)(string) | 제공된 xz 형식 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz)(Stream) | 제공된 Z 형식 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| static [FromZ](../../aspose.zip.tar/tararchive/fromz/#fromz_1)(string) | 제공된 Z 형식 아카이브를 추출하고 구성합니다.`TarArchive` 추출된 데이터에서. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries)(DirectoryInfo, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntries](../../aspose.zip.tar/tararchive/createentries/#createentries_1)(string, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry)(string, FileInfo, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_1)(string, Stream, FileSystemInfo) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.tar/tararchive/createentry/#createentry_2)(string, string, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry_1)(int) | 항목 목록에서 항목을 index. 로 제거합니다. |
| [DeleteEntry](../../aspose.zip.tar/tararchive/deleteentry/#deleteentry)(TarEntry) | 항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다. |
| [Dispose](../../aspose.zip.tar/tararchive/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip.tar/tararchive/extracttodirectory/)(string) | 아카이브의 모든 파일을 제공된 디렉토리에 추출합니다. |
| [Save](../../aspose.zip.tar/tararchive/save/#save)(Stream, TarFormat?) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.tar/tararchive/save/#save_1)(string, TarFormat?) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped)(Stream, TarFormat?) | gzip 압축을 사용하여 아카이브를 스트림에 저장합니다. |
| [SaveGzipped](../../aspose.zip.tar/tararchive/savegzipped/#savegzipped_1)(string, TarFormat?) | gzip 압축을 사용하여 경로별로 아카이브를 파일에 저장합니다. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped)(Stream, TarFormat?) | lzip 압축을 사용하여 아카이브를 스트림에 저장합니다. |
| [SaveLzipped](../../aspose.zip.tar/tararchive/savelzipped/#savelzipped_1)(string, TarFormat?) | lzip 압축을 사용하여 경로별로 아카이브를 파일에 저장합니다. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed)(Stream, TarFormat?, XzArchiveSettings) | xz 압축을 사용하여 아카이브를 스트림에 저장합니다. |
| [SaveXzCompressed](../../aspose.zip.tar/tararchive/savexzcompressed/#savexzcompressed_1)(string, TarFormat?, XzArchiveSettings) | xz 압축을 사용하여 경로별로 아카이브를 경로에 저장합니다. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed)(Stream, TarFormat?) | Z 압축을 사용하여 아카이브를 스트림에 저장합니다. |
| [SaveZCompressed](../../aspose.zip.tar/tararchive/savezcompressed/#savezcompressed_1)(string, TarFormat?) | Z 압축을 사용하여 경로별로 아카이브를 경로에 저장합니다. |

### 또한보십시오

* interface [IArchive](../../aspose.zip/iarchive/)
* 네임스페이스 [Aspose.Zip.Tar](../../aspose.zip.tar/)
* 집회 [Aspose.Zip](../../)


