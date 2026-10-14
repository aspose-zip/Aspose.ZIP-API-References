---
title: "클래스 LhaArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Aspose.Zip.Lha.LhaArchive 클래스. 이 클래스는 LHA .lzh 아카이브 파일을 나타냅니다."
type: docs
weight: 630
url: /ko/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

이 클래스는 LHA (.lzh) 아카이브 파일을 나타냅니다.

```csharp
public class LhaArchive : IArchive
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | 새 `LhaArchive` 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | 새 `LhaArchive` 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | 아카이브를 구성하는 [`LhaArchiveEntry`](../lhaarchiveentry/) 유형의 파일 항목을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | 아카이브에 있는 모든 파일과 디렉터리를 제공된 디렉터리로 추출합니다. |

## 비고

다음 압축 방법만 지원됩니다:

**Method**

**Explanation**

**lh0**

압축되지 않음

**lh4**

8 KiB 슬라이딩 사전 및 정적 Huffman

**lh5**

16 KiB 슬라이딩 사전 및 정적 Huffman

**lh6**

64 KiB 슬라이딩 사전 및 정적 Huffman

**lh7**

128 KiB 슬라이딩 사전 및 정적 Huffman

**lhx**

1 Mib 슬라이딩 사전 및 정적 Huffman

**lhd**

디렉터리

### 또 보기

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


