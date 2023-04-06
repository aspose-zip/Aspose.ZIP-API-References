---
title: Class ArchiveEntryPlain
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.ArchiveEntryPlain 수업. 암호화 없이 압축하거나 복호화 없이 압축을 풀어야 하는 Zip 항목입니다.
type: docs
weight: 40
url: /ko/net/aspose.zip/archiveentryplain/
---
## ArchiveEntryPlain class

암호화 없이 압축하거나 복호화 없이 압축을 풀어야 하는 Zip 항목입니다.

```csharp
public sealed class ArchiveEntryPlain : ArchiveEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Comment](../../aspose.zip/archiveentry/comment/) { get; } | 아카이브 내의 항목에 대한 설명을 가져옵니다. |
| [CompressedSize](../../aspose.zip/archiveentry/compressedsize/) { get; } | 압축 파일의 크기를 가져옵니다. |
| [CompressionSettings](../../aspose.zip/archiveentry/compressionsettings/) { get; } | 압축 또는 압축 해제 설정을 가져옵니다. |
| [IsDirectory](../../aspose.zip/archiveentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [ModificationTime](../../aspose.zip/archiveentry/modificationtime/) { get; set; } | 마지막으로 수정한 날짜와 시간을 가져오거나 설정합니다. |
| [Name](../../aspose.zip/archiveentry/name/) { get; } | 아카이브 내의 항목 이름을 가져옵니다. |
| [UncompressedSize](../../aspose.zip/archiveentry/uncompressedsize/) { get; } | 원본 파일의 크기를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip/archiveentry/extract/)(Stream, string) | 제공된 스트림에 항목을 추출합니다. |
| [Extract](../../aspose.zip/archiveentry/extract/)(string, string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| [Open](../../aspose.zip/archiveentry/open/)(string) | 추출할 항목을 열고 압축 해제된 항목 내용이 있는 스트림을 제공합니다. |

## 이벤트

| 이름 | 설명 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip/archiveentry/compressionprogressed/) | 원시 스트림의 일부가 압축되면 발생합니다. |
| event [ExtractionProgressed](../../aspose.zip/archiveentry/extractionprogressed/) | 원시 스트림의 일부가 추출되면 발생합니다. |

### 또한보십시오

* class [ArchiveEntry](../archiveentry/)
* 네임스페이스 [Aspose.Zip](../../aspose.zip/)
* 집회 [Aspose.Zip](../../)


