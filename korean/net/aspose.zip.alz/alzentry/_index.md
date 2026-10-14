---
title: "클래스 AlzEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Alz.AlzEntry 클래스. 모든 메타데이터와 함께 ALZ 아카이브의 파일 항목을 나타냅니다."
type: docs
weight: 30
url: /ko/net/aspose.zip.alz/alzentry/
---
## AlzEntry class

ALZ 아카이브 내 파일 항목을 모든 메타데이터와 함께 나타냅니다.

```csharp
public abstract class AlzEntry : IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CompressedSize](../../aspose.zip.alz/alzentry/compressedsize/) { get; } | 파일 데이터의 압축된 크기(바이트). |
| [IsDirectory](../../aspose.zip.alz/alzentry/isdirectory/) { get; } | 이 항목이 디렉터리를 나타내면 true를 반환합니다. |
| [Length](../../aspose.zip.alz/alzentry/length/) { get; } |  |
| [Name](../../aspose.zip.alz/alzentry/name/) { get; } | 파일 이름(경로 제외). |
| [UncompressedSize](../../aspose.zip.alz/alzentry/uncompressedsize/) { get; } | 파일 데이터의 압축 해제된 크기(바이트). |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract_1)(Stream, string) | 제공된 스트림으로 항목을 추출합니다. |
| [Extract](../../aspose.zip.alz/alzentry/extract/#extract)(string, string) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | 항목을 추출하기 위해 열고, 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |

### 또 보기

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


