---
title: "클래스 EggEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Egg.EggEntry class. EGG 아카이브 내 파일 항목을 모든 메타데이터와 함께 나타냅니다"
type: docs
weight: 470
url: /ko/net/aspose.zip.egg/eggentry/
---
## EggEntry class

EGG 아카이브 내 파일 항목을 모든 메타데이터와 함께 나타냅니다.

```csharp
public abstract class EggEntry : IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CompressedSize](../../aspose.zip.egg/eggentry/compressedsize/) { get; } | 항목의 압축된 크기를 가져옵니다. |
| [IsDirectory](../../aspose.zip.egg/eggentry/isdirectory/) { get; } | 이 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [Length](../../aspose.zip.egg/eggentry/length/) { get; } |  |
| [ModificationTime](../../aspose.zip.egg/eggentry/modificationtime/) { get; } | 마지막 수정 날짜와 시간을 가져오거나 설정합니다. |
| [Name](../../aspose.zip.egg/eggentry/name/) { get; } | 아카이브 내 항목의 이름을 가져옵니다. |
| [UncompressedSize](../../aspose.zip.egg/eggentry/uncompressedsize/) { get; } | 항목의 압축 해제된 크기를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract_1)(Stream) | 제공된 스트림으로 항목을 추출합니다. |
| [Extract](../../aspose.zip.egg/eggentry/extract/#extract)(string) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [Open](../../aspose.zip.egg/eggentry/open/)() | 항목을 추출하기 위해 열고, 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |

### 또 보기

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Egg](../../aspose.zip.egg/)
* assembly [Aspose.Zip](../../)


