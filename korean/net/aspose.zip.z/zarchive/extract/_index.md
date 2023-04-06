---
title: ZArchive.Extract
second_title: .NET API 참조용 Aspose.ZIP
description: ZArchive 방법. Z 아카이브를 스트림으로 추출합니다.
type: docs
weight: 30
url: /ko/net/aspose.zip.z/zarchive/extract/
---
## Extract(Stream) {#extract_2}

Z 아카이브를 스트림으로 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destination | Stream | 압축 해제된 데이터를 저장하기 위한 스트림. |

### 예외

| 예외 | 상태 |
| --- | --- |
| InvalidDataException | 데이터를 압축 해제할 수 없습니다. |

### 예

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (FileStream extractedFile = File.Open(extractedFileName, FileMode.Create))
    {
        using (var archive = new ZArchive(zFile))
        {
            archive.Extract(extractedFile);
        }
    }
}
```

### 또한보십시오

* class [ZArchive](../)
* 네임스페이스 [Aspose.Zip.Z](../../zarchive/)
* 집회 [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Z 아카이브를 파일로 추출합니다.

```csharp
public void Extract(FileInfo fileInfo)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileInfo | FileInfo | 압축 해제된 데이터를 저장하기 위한 FileInfo. |

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
| InvalidDataException | 데이터를 압축 해제할 수 없습니다. |

### 예

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract(new FileInfo("extracted.bin"));
    }
}
```

### 또한보십시오

* class [ZArchive](../)
* 네임스페이스 [Aspose.Zip.Z](../../zarchive/)
* 집회 [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Z 아카이브를 경로별로 파일로 추출합니다.

```csharp
public FileInfo Extract(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 압축 해제된 데이터를 저장할 파일의 경로입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *path* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*path* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*path* 거부되었습니다. |
| PathTooLongException | 지정된*path*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*path* 문자열 중간에 콜론(:)을 포함합니다. |
| InvalidDataException | 데이터를 압축 해제할 수 없습니다. |

### 예

```csharp
using (FileStream zFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ZArchive(zFile))
    {
        archive.Extract("extracted.bin");
    }
}
```

### 또한보십시오

* class [ZArchive](../)
* 네임스페이스 [Aspose.Zip.Z](../../zarchive/)
* 집회 [Aspose.Zip](../../../)


