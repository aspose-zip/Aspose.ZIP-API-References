---
title: GzipArchive.SetSource
second_title: .NET API 참조용 Aspose.ZIP
description: GzipArchive 방법. 아카이브 내에서 압축할 콘텐츠를 설정합니다.
type: docs
weight: 70
url: /ko/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(Stream source)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| source | Stream | 아카이브의 입력 스트림입니다. |

### 예

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(FileInfo fileInfo)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| fileInfo | FileInfo | 압축할 파일에 대한 참조입니다. |

### 예

스트림에서 아카이브를 열고 압축을 풉니다.`메모리 스트림`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 압축할 파일의 경로입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *path* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*path* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*path* 거부되었습니다. |
| PathTooLongException | 지정된*path*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*path* 문자열 중간에 콜론(:)을 포함합니다. |

### 예

경로로 파일에서 아카이브를 열고 압축을 풉니다.`메모리 스트림`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

아카이브 내에서 압축할 콘텐츠를 설정합니다.

```csharp
public void SetSource(TarArchive tarArchive)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| tarArchive | TarArchive | 압축할 Tar 아카이브입니다. |

### 비고

이 방법을 사용하여 합동 tar.gz 아카이브를 구성합니다.

### 예

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### 또한보십시오

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)


