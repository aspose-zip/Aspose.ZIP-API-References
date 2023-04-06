---
title: Class CpioEntry
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Cpio.CpioEntry 수업. cpio 아카이브 내의 단일 파일을 나타냅니다.
type: docs
weight: 170
url: /ko/net/aspose.zip.cpio/cpioentry/
---
## CpioEntry class

cpio 아카이브 내의 단일 파일을 나타냅니다.

```csharp
public sealed class CpioEntry : IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [IsDirectory](../../aspose.zip.cpio/cpioentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [LastWriteTimeUtc](../../aspose.zip.cpio/cpioentry/lastwritetimeutc/) { get; } | 마지막 쓰기 시간을 가져옵니다. |
| [Length](../../aspose.zip.cpio/cpioentry/length/) { get; } | 항목의 길이를 바이트 단위로 가져옵니다. |
| [Name](../../aspose.zip.cpio/cpioentry/name/) { get; } | 아카이브 내의 항목 이름을 가져옵니다. |
| [Parent](../../aspose.zip.cpio/cpioentry/parent/) { get; } | 항목이 속한 아카이브를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract_1)(Stream) | 제공된 스트림에 항목을 추출합니다. |
| [Extract](../../aspose.zip.cpio/cpioentry/extract/#extract)(string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| [Open](../../aspose.zip.cpio/cpioentry/open/)() | 추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다. |
| override [ToString](../../aspose.zip.cpio/cpioentry/tostring/)() |  |

### 또한보십시오

* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 네임스페이스 [Aspose.Zip.Cpio](../../aspose.zip.cpio/)
* 집회 [Aspose.Zip](../../)


