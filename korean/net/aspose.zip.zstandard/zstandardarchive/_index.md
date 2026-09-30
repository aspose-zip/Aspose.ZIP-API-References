---
title: "ZstandardArchive 클래스"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Zstandard.ZstandardArchive 클래스. 이 클래스는 Zstandard 아카이브 파일을 나타냅니다. Zstandard 아카이브를 구성하는 데 사용합니다"
type: docs
weight: 1620
url: /ko/net/aspose.zip.zstandard/zstandardarchive/
---
## ZstandardArchive class

이 클래스는 Zstandard 아카이브 파일을 나타냅니다. 이를 사용하여 Zstandard 아카이브를 구성할 수 있습니다.

```csharp
public class ZstandardArchive : IArchive, IArchiveFileEntry
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ZstandardArchive](zstandardarchive/#constructor)() | `ZstandardArchive` 클래스의 새 인스턴스를 초기화합니다(압축을 위해 준비됨). |
| [ZstandardArchive](zstandardarchive/#constructor_1)(Stream, ZstandardLoadOptions) | `ZstandardArchive` 클래스의 새 인스턴스를 초기화합니다(압축 해제를 위해 준비됨). |
| [ZstandardArchive](zstandardarchive/#constructor_2)(string, ZstandardLoadOptions) | `ZstandardArchive` 클래스의 새 인스턴스를 초기화합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Dispose](../../aspose.zip.zstandard/zstandardarchive/dispose/)() | 관리되지 않는 리소스를 해제, 릴리스 또는 재설정과 관련된 애플리케이션 정의 작업을 수행합니다. |
| [Extract](../../aspose.zip.zstandard/zstandardarchive/extract/#extract_1)(Stream) | 제공된 스트림으로 아카이브를 추출합니다. |
| [Extract](../../aspose.zip.zstandard/zstandardarchive/extract/#extract)(string) | 경로를 지정하여 파일로 아카이브를 추출합니다. |
| [ExtractToDirectory](../../aspose.zip.zstandard/zstandardarchive/extracttodirectory/)(string) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [Open](../../aspose.zip.zstandard/zstandardarchive/open/)() | 아카이브를 추출하기 위해 열고 아카이브 콘텐츠가 포함된 스트림을 제공합니다. |
| [Save](../../aspose.zip.zstandard/zstandardarchive/save/#save)(FileInfo, ZstandardSaveOptions) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.zstandard/zstandardarchive/save/#save_1)(Stream, ZstandardSaveOptions) | 제공된 스트림에 아카이브를 저장합니다. |
| [Save](../../aspose.zip.zstandard/zstandardarchive/save/#save_2)(string, ZstandardSaveOptions) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [SetSource](../../aspose.zip.zstandard/zstandardarchive/setsource/#setsource)(FileInfo) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [SetSource](../../aspose.zip.zstandard/zstandardarchive/setsource/#setsource_1)(Stream) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [SetSource](../../aspose.zip.zstandard/zstandardarchive/setsource/#setsource_2)(string) | 아카이브 내에서 압축될 내용을 설정합니다. |

### 또 보기

* interface [IArchive](../../aspose.zip/iarchive/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* namespace [Aspose.Zip.Zstandard](../../aspose.zip.zstandard/)
* assembly [Aspose.Zip](../../)


