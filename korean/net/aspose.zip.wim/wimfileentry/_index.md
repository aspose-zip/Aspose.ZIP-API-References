---
title: Class WimFileEntry
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Wim.WimFileEntry 수업. wim 아카이브 내의 단일 파일을 나타냅니다.
type: docs
weight: 790
url: /ko/net/aspose.zip.wim/wimfileentry/
---
## WimFileEntry class

wim 아카이브 내의 단일 파일을 나타냅니다.

```csharp
public sealed class WimFileEntry : WimEntry, IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [AlternateDataStreams](../../aspose.zip.wim/wimentry/alternatedatastreams/) { get; } | 파일 또는 디렉터리에 대한 대체 데이터 스트림의 이름을 가져옵니다. |
| [Archive](../../aspose.zip.wim/wimentry/archive/) { get; } | 항목이 속한 아카이브를 가져옵니다. |
| [ChangeTime](../../aspose.zip.wim/wimentry/changetime/) { get; } | 파일 또는 디렉터리가 마지막으로 변경된 시간을 가져옵니다. |
| [CreationTime](../../aspose.zip.wim/wimentry/creationtime/) { get; } | 파일 또는 디렉터리의 생성 시간을 가져옵니다. |
| [FileAttributes](../../aspose.zip.wim/wimentry/fileattributes/) { get; } | 파일 또는 디렉터리 특성을 가져옵니다. |
| [FullPath](../../aspose.zip.wim/wimentry/fullpath/) { get; } | 이미지 내 항목의 전체 경로를 가져옵니다. |
| [HardLink](../../aspose.zip.wim/wimentry/hardlink/) { get; } | 파일 또는 디렉터리의 하드링크 ID를 가져옵니다. |
| [HasHardLinks](../../aspose.zip.wim/wimentry/hashardlinks/) { get; } | 파일 또는 디렉터리가 다른 이름으로 알려져 있는지 여부를 가져옵니다. |
| [Image](../../aspose.zip.wim/wimentry/image/) { get; } | 항목이 속한 이미지를 가져옵니다. |
| [IsDirectory](../../aspose.zip.wim/wimentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [LastAccessTime](../../aspose.zip.wim/wimentry/lastaccesstime/) { get; } | 파일 또는 디렉터리의 마지막 액세스 시간을 가져옵니다. |
| [LastWriteTime](../../aspose.zip.wim/wimentry/lastwritetime/) { get; } | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| [Length](../../aspose.zip.wim/wimfileentry/length/) { get; } | 항목의 길이를 바이트 단위로 가져옵니다. |
| [Name](../../aspose.zip.wim/wimentry/name/) { get; } | 이미지 내의 항목 이름을 가져옵니다. |
| [Parent](../../aspose.zip.wim/wimentry/parent/) { get; } | 항목이 속한 상위 디렉토리를 가져옵니다. |
| [ShortName](../../aspose.zip.wim/wimentry/shortname/) { get; } | 이미지 내 항목의 짧은 이름을 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract_1)(Stream) | 제공된 스트림에 항목을 추출합니다. |
| [Extract](../../aspose.zip.wim/wimfileentry/extract/#extract)(string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| [Open](../../aspose.zip.wim/wimfileentry/open/)() | 추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다. |
| override [ToString](../../aspose.zip.wim/wimentry/tostring/)() |  |

### 또한보십시오

* class [WimEntry](../wimentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 네임스페이스 [Aspose.Zip.Wim](../../aspose.zip.wim/)
* 집회 [Aspose.Zip](../../)


