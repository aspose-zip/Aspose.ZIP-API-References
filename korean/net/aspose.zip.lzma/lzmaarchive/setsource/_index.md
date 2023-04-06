---
title: LzmaArchive.SetSource
second_title: .NET API 참조용 Aspose.ZIP
description: LzmaArchive 방법. 아카이브 내에서 압축할 콘텐츠를 설정합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip.lzma/lzmaarchive/setsource/
---
## SetSource(Stream) {#setsource_1}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(Stream source)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| source | Stream | 아카이브의 입력 스트림입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | 그만큼*source* 스트림을 찾을 수 없습니다. |

### 예

```csharp
using (var archive = new LzmaArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lzma");
}
```

### 또한보십시오

* class [LzmaArchive](../)
* 네임스페이스 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 집회 [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(FileInfo fileInfo)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileInfo | FileInfo | 입력 스트림으로 열리는 FileInfo. |

### 예외

| 예외 | 상태 |
| --- | --- |
| SecurityException | 호출자에게 파일을 여는 데 필요한 권한이 없습니다.*fileInfo*. |
| ArgumentException | 파일 경로가 비어 있거나 공백만 포함되어 있습니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| UnauthorizedAccessException | 파일 경로가 읽기 전용이거나 디렉토리입니다. |
| ArgumentNullException | *fileInfo* null입니다. |
| DirectoryNotFoundException | 매핑되지 않은 드라이브에 있는 것과 같이 지정된 경로가 잘못되었습니다. |
| IOException | 파일이 이미 열려 있습니다. |

### 예

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lzma");
}
```

### 또한보십시오

* class [LzmaArchive](../)
* 네임스페이스 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 집회 [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(string sourcePath)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourcePath | String | 입력 스트림으로 열릴 파일의 경로입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *sourcePath* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*sourcePath* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*sourcePath* 거부되었습니다. |
| PathTooLongException | 지정된*sourcePath*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*sourcePath* 문자열 중간에 콜론(:)을 포함합니다. |

### 예

```csharp
using (var archive = new LzmaArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lzma");
}
```

### 또한보십시오

* class [LzmaArchive](../)
* 네임스페이스 [Aspose.Zip.LZMA](../../lzmaarchive/)
* 집회 [Aspose.Zip](../../../)


