---
title: "클래스 IsoArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Iso.IsoArchive 클래스. ISO 9660 ISO 아카이브를 나타냅니다."
type: docs
weight: 570
url: /ko/net/aspose.zip.iso/isoarchive/
---
## IsoArchive class

ISO 아카이브 (ISO 9660)를 나타냅니다.

```csharp
public sealed class IsoArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [IsoArchive](isoarchive/#constructor)() | `IsoArchive` 클래스의 새 인스턴스를 초기화하고 새 파일 및 디렉터리를 추가하기 위한 빈 ISO 아카이브를 생성합니다. |
| [IsoArchive](isoarchive/#constructor_1)(Stream, IsoLoadOptions) | `IsoArchive` 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [IsoArchive](isoarchive/#constructor_2)(string, IsoLoadOptions) | `IsoArchive` 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.iso/isoarchive/entries/) { get; } | 아카이브를 구성하는 [`IsoEntry`](../isoentry/) 유형의 항목을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CreateDirectory](../../aspose.zip.iso/isoarchive/createdirectory/)(string) | ISO 이미지에 디렉터리를 추가합니다. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry)(string) | ISO 이미지에 파일을 추가합니다. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_1)(string, Stream) | ISO 이미지에 파일을 추가합니다. |
| [CreateEntry](../../aspose.zip.iso/isoarchive/createentry/#createentry_2)(string, string) | ISO 이미지에 파일을 추가합니다. |
| [Dispose](../../aspose.zip.iso/isoarchive/dispose/)() | 관리되지 않는 리소스를 해제, 릴리스 또는 재설정과 관련된 애플리케이션 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip.iso/isoarchive/extracttodirectory/)(string) | 지정된 디렉터리로 모든 항목을 추출합니다. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save)(Stream, IsoSaveOptions) | ISO 이미지를 지정된 스트림에 저장합니다. |
| [Save](../../aspose.zip.iso/isoarchive/save/#save_1)(string, IsoSaveOptions) | ISO 이미지를 지정된 경로에 저장합니다. |

### 또 보기

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Iso](../../aspose.zip.iso/)
* assembly [Aspose.Zip](../../)


