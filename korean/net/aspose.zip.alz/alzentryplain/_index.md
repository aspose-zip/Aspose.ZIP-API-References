---
title: "클래스 AlzEntryPlain"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Alz.AlzEntryPlain 클래스. 복호화 없이 압축 해제해야 하는 ALZ 항목"
type: docs
weight: 50
url: /ko/net/aspose.zip.alz/alzentryplain/
---
## AlzEntryPlain class

복호화 없이 압축 해제해야 하는 ALZ 항목입니다.

```csharp
public sealed class AlzEntryPlain : AlzEntry
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
| [Extract](../../aspose.zip.alz/alzentry/extract/)(Stream, string) | 제공된 스트림으로 항목을 추출합니다. |
| [Extract](../../aspose.zip.alz/alzentry/extract/)(string, string) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [Open](../../aspose.zip.alz/alzentry/open/)(string) | 항목을 추출하기 위해 열고, 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |

### 또 보기

* class [AlzEntry](../alzentry/)
* namespace [Aspose.Zip.Alz](../../aspose.zip.alz/)
* assembly [Aspose.Zip](../../)


