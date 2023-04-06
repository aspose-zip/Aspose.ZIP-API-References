---
title: Class GzipArchive
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Gzip.GzipArchive 수업. 이 클래스는 gzip 아카이브 파일을 나타냅니다. gzip 아카이브를 작성하거나 추출하는 데 사용하십시오.
type: docs
weight: 210
url: /ko/net/aspose.zip.gzip/gziparchive/
---
## GzipArchive class

이 클래스는 gzip 아카이브 파일을 나타냅니다. gzip 아카이브를 작성하거나 추출하는 데 사용하십시오.

```csharp
public class GzipArchive : IArchive, IArchiveFileEntry
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [GzipArchive](gziparchive/#constructor)() | 의 새 인스턴스를 초기화합니다.`GzipArchive` 압축을 위해 준비된 클래스. |
| [GzipArchive](gziparchive/#constructor_1)(Stream, bool) | 의 새 인스턴스를 초기화합니다.`GzipArchive` 압축 해제를 위해 준비된 클래스. |
| [GzipArchive](gziparchive/#constructor_2)(string, bool) | 의 새 인스턴스를 초기화합니다.`GzipArchive` 클래스. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Name](../../aspose.zip.gzip/gziparchive/name/) { get; } | 원본 파일의 이름. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Dispose](../../aspose.zip.gzip/gziparchive/dispose/)() | 관리되지 않는 리소스 해제, 해제 또는 재설정과 관련된 응용 프로그램 정의 작업을 수행합니다. |
| [Extract](../../aspose.zip.gzip/gziparchive/extract/)(Stream) | 제공된 스트림에 아카이브를 추출합니다. |
| [Open](../../aspose.zip.gzip/gziparchive/open/)() | 추출을 위해 아카이브를 열고 아카이브 콘텐츠가 있는 스트림을 제공합니다. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save)(Stream) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.gzip/gziparchive/save/#save_1)(string) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_1)(FileInfo) | 아카이브 내에서 압축할 콘텐츠를 설정합니다. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_2)(Stream) | 아카이브 내에서 압축할 콘텐츠를 설정합니다. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource_3)(string) | 아카이브 내에서 압축할 콘텐츠를 설정합니다. |
| [SetSource](../../aspose.zip.gzip/gziparchive/setsource/#setsource)(TarArchive) | 아카이브 내에서 압축할 콘텐츠를 설정합니다. |

### 비고

Gzip 압축 알고리즘은 LZ77과 Huffman 코딩의 조합인 DEFLATE 알고리즘을 기반으로 합니다.

### 또한보십시오

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 네임스페이스 [Aspose.Zip.Gzip](../../aspose.zip.gzip/)
* 집회 [Aspose.Zip](../../)


