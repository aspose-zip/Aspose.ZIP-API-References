---
title: Class SevenZipArchiveEntry
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.SevenZip.SevenZipArchiveEntry 수업. 7z 아카이브 내의 단일 파일을 나타냅니다.
type: docs
weight: 670
url: /ko/net/aspose.zip.sevenzip/sevenziparchiveentry/
---
## SevenZipArchiveEntry class

7z 아카이브 내의 단일 파일을 나타냅니다.

```csharp
public abstract class SevenZipArchiveEntry : IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/compressedsize/) { get; } | 압축 파일의 크기를 가져옵니다. |
| [CompressionSettings](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionsettings/) { get; } | 압축 또는 압축 해제 설정을 가져옵니다. |
| [IsDirectory](../../aspose.zip.sevenzip/sevenziparchiveentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [ModificationTime](../../aspose.zip.sevenzip/sevenziparchiveentry/modificationtime/) { get; } | 마지막으로 수정한 날짜와 시간을 가져옵니다. |
| [Name](../../aspose.zip.sevenzip/sevenziparchiveentry/name/) { get; } | 아카이브 내의 항목 이름을 가져옵니다. |
| [UncompressedSize](../../aspose.zip.sevenzip/sevenziparchiveentry/uncompressedsize/) { get; } | 원본 파일의 크기를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract_1)(Stream, string) | 제공된 스트림에 항목을 추출합니다. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/#extract)(string, string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | 추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다. |

## 이벤트

| 이름 | 설명 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | 원시 스트림의 일부가 압축되면 발생합니다. |

### 비고

캐스팅`SevenZipArchiveEntry` 인스턴스[`SevenZipArchiveEntryEncrypted`](../sevenziparchiveentryencrypted/) 항목이 암호화되었는지 여부를 결정합니다.

### 또한보십시오

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 네임스페이스 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* 집회 [Aspose.Zip](../../)


