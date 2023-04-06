---
title: Class XarFileEntry
second_title: .NET API 참조용 Aspose.ZIP
description: Aspose.Zip.Xar.XarFileEntry 수업. xar 아카이브 내의 파일 항목을 나타냅니다.
type: docs
weight: 840
url: /ko/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

xar 아카이브 내의 파일 항목을 나타냅니다.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | 파일 또는 디렉터리의 생성 시간을 가져옵니다. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | 아카이브 내 항목의 전체 경로를 가져옵니다. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | 파일 또는 디렉터리의 마지막 액세스 시간을 가져옵니다. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | 항목의 길이를 바이트 단위로 가져옵니다. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | 아카이브 내의 항목 이름을 가져옵니다. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | 항목이 속한 상위 디렉토리를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | 제공된 스트림에 항목을 추출합니다. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | 제공된 경로로 항목을 파일 시스템으로 추출합니다. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | 추출할 항목을 열고 항목 내용이 있는 스트림을 제공합니다. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### 또한보십시오

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* 네임스페이스 [Aspose.Zip.Xar](../../aspose.zip.xar/)
* 집회 [Aspose.Zip](../../)


