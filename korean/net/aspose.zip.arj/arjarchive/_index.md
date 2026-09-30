---
title: "클래스 ArjArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Arj.ArjArchive 클래스. 이 클래스는 ARJ 아카이브 파일을 나타냅니다."
type: docs
weight: 250
url: /ko/net/aspose.zip.arj/arjarchive/
---
## ArjArchive class

이 클래스는 ARJ 아카이브 파일을 나타냅니다.

```csharp
public class ArjArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ArjArchive](arjarchive/#constructor)(Stream, ArjLoadOptions) | 새 인스턴스를 초기화합니다 `ArjArchive` 클래스의 새 인스턴스를 만들고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [ArjArchive](arjarchive/#constructor_1)(string, ArjLoadOptions) | 새 인스턴스를 초기화합니다 `ArjArchive` 클래스의 새 인스턴스를 만들고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Commentary](../../aspose.zip.arj/arjarchive/commentary/) { get; } | 주석을 가져옵니다. |
| [Entries](../../aspose.zip.arj/arjarchive/entries/) { get; } | ARJ 아카이브를 구성하는 [`ArjEntryPlain`](../arjentryplain/) 유형의 항목을 가져옵니다. |
| [Name](../../aspose.zip.arj/arjarchive/name/) { get; } | 원래 이름을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Dispose](../../aspose.zip.arj/arjarchive/dispose/)() | 관리되지 않는 리소스를 해제, 릴리스 또는 재설정과 관련된 애플리케이션 정의 작업을 수행합니다. |
| [ExtractToDirectory](../../aspose.zip.arj/arjarchive/extracttodirectory/)(string) | 지정된 디렉터리로 모든 항목을 추출합니다. |

## 비고

다음 압축 방법만 지원됩니다:

**Method**

**Explanation**

**0**

압축되지 않음

**1**

LZ77과 적응형 허프만 코딩의 조합. 최고의 압축 비율.

**2**

LZ77과 적응형 허프만 코딩의 조합.

**3**

LZ77과 적응형 허프만 코딩의 조합. 최고의 속도.

### 또 보기

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Arj](../../aspose.zip.arj/)
* assembly [Aspose.Zip](../../)


