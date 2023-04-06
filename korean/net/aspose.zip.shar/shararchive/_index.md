---
title: Class SharArchive
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Shar.SharArchive 수업. 이 클래스는 공유 아카이브 파일을 나타냅니다.
type: docs
weight: 700
url: /ko/net/aspose.zip.shar/shararchive/
---
## SharArchive class

이 클래스는 공유 아카이브 파일을 나타냅니다.

```csharp
public class SharArchive : IDisposable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [SharArchive](shararchive/#constructor)() | 의 새 인스턴스를 초기화합니다.`SharArchive` 클래스. |
| [SharArchive](shararchive/#constructor_1)(string) |  |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.shar/shararchive/entries/) { get; } | 항목 가져오기[`SharEntry`](../sharentry/) 아카이브를 구성하는 유형. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries)(DirectoryInfo, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntries](../../aspose.zip.shar/shararchive/createentries/#createentries_1)(string, bool) | 지정된 디렉토리에 재귀적으로 모든 파일과 디렉토리를 아카이브에 추가합니다. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_1)(string, Stream) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry)(string, FileInfo, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [CreateEntry](../../aspose.zip.shar/shararchive/createentry/#createentry_2)(string, string, bool) | 아카이브 내에 단일 항목을 생성합니다. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry_1)(int) | 항목 목록에서 항목을 index. 로 제거합니다. |
| [DeleteEntry](../../aspose.zip.shar/shararchive/deleteentry/#deleteentry)(SharEntry) | 항목 목록에서 특정 항목의 첫 번째 항목을 제거합니다. |
| [Dispose](../../aspose.zip.shar/shararchive/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [Save](../../aspose.zip.shar/shararchive/save/#save)(Stream) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.shar/shararchive/save/#save_1)(string) | 제공된 대상 파일에 아카이브를 저장합니다. |

### 또한보십시오

* 네임스페이스 [Aspose.Zip.Shar](../../aspose.zip.shar/)
* 집회 [Aspose.Zip](../../)


