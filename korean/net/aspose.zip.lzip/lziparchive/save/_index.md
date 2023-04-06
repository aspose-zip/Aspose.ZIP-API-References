---
title: LzipArchive.Save
second_title: .NET API 참조용 Aspose.ZIP
description: LzipArchive 방법. 제공된 스트림에 lzip 아카이브를 저장합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip.lzip/lziparchive/save/
---
## Save(Stream) {#save_1}

제공된 스트림에 lzip 아카이브를 저장합니다.

```csharp
public void Save(Stream outputStream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| outputStream | Stream | 대상 스트림. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *outputStream* 찾기를 지원하지 않습니다. |
| ArgumentNullException | *outputStream* null입니다. |

### 비고

*outputStream* 검색 가능해야 합니다.

### 예

```csharp
using (FileStream lzFile = File.Open("archive.lz", FileMode.Create))
{
    using (var archive = new LzipArchive())
    {
        archive.SetSource("data.bin");
        archive.Save(lzFile);
     }
}
```

### 또한보십시오

* class [LzipArchive](../)
* 네임스페이스 [Aspose.Zip.Lzip](../../lziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

제공된 대상 파일에 lzip 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *destinationFileName* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*destinationFileName* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*destinationFileName* 거부되었습니다. |
| PathTooLongException | 지정된*destinationFileName*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*destinationFileName* 문자열 중간에 콜론(:)을 포함합니다. |

### 예

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.lz");
}
```

### 또한보십시오

* class [LzipArchive](../)
* 네임스페이스 [Aspose.Zip.Lzip](../../lziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

제공된 대상 파일에 lzip 아카이브를 저장합니다.

```csharp
public void Save(FileInfo destination)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destination | FileInfo | 대상 스트림으로 열릴 FileInfo입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| SecurityException | 호출자에게 파일을 여는 데 필요한 권한이 없습니다.*destination*. |
| ArgumentException | 파일 경로가 비어 있거나 공백만 포함되어 있습니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| UnauthorizedAccessException | 파일 경로가 읽기 전용이거나 디렉토리입니다. |
| ArgumentNullException | *destination* null입니다. |
| DirectoryNotFoundException | 매핑되지 않은 드라이브에 있는 것과 같이 지정된 경로가 잘못되었습니다. |
| IOException | 파일이 이미 열려 있습니다. |

### 예

```csharp
using (var archive = new LzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz"));
}
```

### 또한보십시오

* class [LzipArchive](../)
* 네임스페이스 [Aspose.Zip.Lzip](../../lziparchive/)
* 집회 [Aspose.Zip](../../../)


