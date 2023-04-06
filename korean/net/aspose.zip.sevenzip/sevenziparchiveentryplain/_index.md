---
title: Class SevenZipArchiveEntryPlain
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.SevenZip.SevenZipArchiveEntryPlain 수업. 암호화 없이 압축하거나 복호화 없이 압축 해제해야 하는 SevenZip 항목입니다.
type: docs
weight: 690
url: /ko/net/aspose.zip.sevenzip/sevenziparchiveentryplain/
---
## SevenZipArchiveEntryPlain class

암호화 없이 압축하거나 복호화 없이 압축 해제해야 하는 SevenZip 항목입니다.

```csharp
public class SevenZipArchiveEntryPlain : SevenZipArchiveEntry
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
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(Stream, string) | 제공된 스트림에 항목을 추출합니다. |
| [Extract](../../aspose.zip.sevenzip/sevenziparchiveentry/extract/)(string, string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| [Open](../../aspose.zip.sevenzip/sevenziparchiveentry/open/)(string) | 추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다. |

## 이벤트

| 이름 | 설명 |
| --- | --- |
| event [CompressionProgressed](../../aspose.zip.sevenzip/sevenziparchiveentry/compressionprogressed/) | 원시 스트림의 일부가 압축되면 발생합니다. |

### 또한보십시오

* class [SevenZipArchiveEntry](../sevenziparchiveentry/)
* 네임스페이스 [Aspose.Zip.SevenZip](../../aspose.zip.sevenzip/)
* 집회 [Aspose.Zip](../../)


