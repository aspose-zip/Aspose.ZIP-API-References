---
title: "ArchiveFactory.CompressDirectory"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ArchiveFactory 메서드. 지정된 디렉터리를 제공된 아카이브 형식을 사용하여 아카이브 파일로 압축합니다"
type: docs
weight: 10
url: /ko/net/aspose.zip/archivefactory/compressdirectory/
---
## ArchiveFactory.CompressDirectory method

제공된 아카이브 형식을 사용하여 지정된 디렉터리를 아카이브 파일로 압축합니다.

```csharp
public static void CompressDirectory(string path, string outputFileName, 
    ArchiveFormat archiveFormat)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 압축될 디렉터리의 경로. |
| outputFileName | String | 대상 파일 이름. |
| archiveFormat | ArchiveFormat | 생성할 아카이브 형식 (예: zip, rar, tar 등). |

### 예외

| 예외 | 조건 |
| --- | --- |
| DirectoryNotFoundException | *path*에 지정된 디렉터리가 존재하지 않을 경우 발생합니다. |
| ArgumentException | *path*가 null이거나 빈 문자열일 경우 발생합니다. |
| NotSupportedException | 지정된 *archiveFormat*이 지원되지 않거나 인식되지 않을 경우 발생합니다. |
| ArgumentNullException | *path*는 `null`입니다. |

## 비고

이 메서드는 *path* 매개변수로 지정된 위치에 아카이브 파일을 생성합니다. 아카이브 파일 이름은 일반적으로 디렉터리 이름에 *archiveFormat*에 따라 적절한 파일 확장자를 붙인 형태가 됩니다. 디렉터리 자체는 수정되거나 삭제되지 않습니다.

## 예제

CompressDirectory 메서드를 사용하는 예시입니다:

```csharp
string directoryPath = @"C:\path\to\your\directory";
ArchiveInfo.ArchiveFormat format = ArchiveInfo.ArchiveFormat.Zip;
ArchiveFactory.CompressDirectory(directoryPath, "result", format);
// 지정된 경로에 있는 디렉터리의 내용을 포함한 ZIP 파일을 생성합니다.
```

### 또 보기

* enum [ArchiveFormat](../../../aspose.zip.archiveinfo/archiveformat/)
* class [ArchiveFactory](../)
* namespace [Aspose.Zip](../../archivefactory/)
* assembly [Aspose.Zip](../../../)


