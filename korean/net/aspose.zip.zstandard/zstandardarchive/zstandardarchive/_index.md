---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ZstandardArchive 생성자. 압축을 위해 준비된 ZstandardArchive 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

압축을 위해 준비된 [`ZstandardArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ZstandardArchive()
```

## 예제

다음 예제는 파일을 압축하는 방법을 보여줍니다.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### 또 보기

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

압축 해제를 위해 준비된 [`ZstandardArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceStream | 스트림 | 아카이브의 소스입니다. |
| 옵션 | ZstandardLoadOptions | 아카이브를 로드할 옵션입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| EndOfStreamException | 스트림의 끝에 예기치 않게 도달했을 때 발생합니다. |
| IOException | I/O 오류가 발생했습니다. |
| InvalidDataException | 데이터가 유효하지 않거나 손상된 경우에 발생합니다. |

## 비고

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [`Open`](../open/) 메서드를 참조하십시오.

## 예제

스트림에서 아카이브를 열고 `MemoryStream`에 추출합니다.

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### 또 보기

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

[`ZstandardArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일의 경로입니다. |
| 옵션 | ZstandardLoadOptions | 아카이브를 로드할 옵션입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| EndOfStreamException | 스트림의 끝에 예기치 않게 도달했을 때 발생합니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| IOException | 파일이 이미 열려 있습니다. |
| InvalidDataException | 데이터가 유효하지 않거나 손상된 경우에 발생합니다. |

## 비고

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [`Open`](../open/) 메서드를 참조하십시오.

## 예제

경로를 통해 파일에서 아카이브를 열고 `MemoryStream`에 추출합니다.

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### 또 보기

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


