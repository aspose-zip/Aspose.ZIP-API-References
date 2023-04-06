---
title: Class RarArchiveEntryPlain
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Rar.RarArchiveEntryPlain 수업. 복호화 없이 압축을 풀어야 하는 RAR 항목.
type: docs
weight: 340
url: /ko/net/aspose.zip.rar/rararchiveentryplain/
---
## RarArchiveEntryPlain class

복호화 없이 압축을 풀어야 하는 RAR 항목.

```csharp
public sealed class RarArchiveEntryPlain : RarArchiveEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CompressedSize](../../aspose.zip.rar/rararchiveentry/compressedsize/) { get; } | 압축 파일의 크기를 가져옵니다. |
| [CreationTime](../../aspose.zip.rar/rararchiveentry/creationtime/) { get; } | 생성 날짜 및 시간을 가져옵니다. |
| [IsDirectory](../../aspose.zip.rar/rararchiveentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [LastAccessTime](../../aspose.zip.rar/rararchiveentry/lastaccesstime/) { get; } | 마지막 액세스 날짜 및 시간을 가져옵니다. |
| [ModificationTime](../../aspose.zip.rar/rararchiveentry/modificationtime/) { get; } | 마지막으로 수정한 날짜와 시간을 가져옵니다. |
| [Name](../../aspose.zip.rar/rararchiveentry/name/) { get; } | 아카이브 내의 항목 이름을 가져옵니다. |
| [UncompressedSize](../../aspose.zip.rar/rararchiveentry/uncompressedsize/) { get; } | 원본 파일의 크기를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(Stream, string) | 제공된 스트림에 항목을 추출합니다. |
| [Extract](../../aspose.zip.rar/rararchiveentry/extract/)(string, string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| [Open](../../aspose.zip.rar/rararchiveentry/open/)(string) | 추출할 항목을 열고 압축 해제된 항목 내용이 있는 스트림을 제공합니다. |

## 이벤트

| 이름 | 설명 |
| --- | --- |
| event [ExtractionProgressed](../../aspose.zip.rar/rararchiveentry/extractionprogressed/) | 원시 스트림의 일부가 추출되면 발생합니다. |

### 또한보십시오

* class [RarArchiveEntry](../rararchiveentry/)
* 네임스페이스 [Aspose.Zip.Rar](../../aspose.zip.rar/)
* 집회 [Aspose.Zip](../../)


