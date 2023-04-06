---
title: GzipArchive.GzipArchive
second_title: .NET API 참조용 Aspose.ZIP
description: GzipArchive 건설자. 의 새 인스턴스를 초기화합니다.GzipArchive 압축을 위해 준비된 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.gzip/gziparchive/gziparchive/
---
## GzipArchive() {#constructor}

의 새 인스턴스를 초기화합니다.[`GzipArchive`](../) 압축을 위해 준비된 클래스.

```csharp
public GzipArchive()
```

### 예

다음 예제는 파일을 압축하는 방법을 보여줍니다.

```csharp
using (GzipArchive archive = new GzipArchive()) 
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

## GzipArchive(Stream, bool) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`GzipArchive`](../) 압축 해제를 위해 준비된 클래스.

```csharp
public GzipArchive(Stream sourceStream, bool parseHeader = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | Stream | 아카이브의 소스입니다. |
| parseHeader | Boolean | 이름을 포함한 속성을 파악하기 위해 스트림 헤더를 구문 분석할지 여부입니다. 검색 가능한 스트림에만 적합합니다. |

### 비고

이 생성자는 압축을 풀지 않습니다. 보다[`Open`](../open/) 압축 해제 방법.

### 예

스트림에서 아카이브를 열고 압축을 풉니다.`메모리 스트림`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive(File.OpenRead("archive.gz")))
  archive.Open().CopyTo(ms);
```

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## GzipArchive(string, bool) {#constructor_2}

의 새 인스턴스를 초기화합니다.[`GzipArchive`](../) 클래스.

```csharp
public GzipArchive(string path, bool parseHeader = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 아카이브 파일의 경로입니다. |
| parseHeader | Boolean | 이름을 포함한 속성을 파악하기 위해 스트림 헤더를 구문 분석할지 여부입니다. 검색 가능한 스트림에만 적합합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *path* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*path* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*path* 거부되었습니다. |
| PathTooLongException | 지정된*path*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*path* 문자열 중간에 콜론(:)을 포함합니다. |

### 비고

이 생성자는 압축을 풀지 않습니다. 보다[`Open`](../open/) 압축 해제 방법.

### 예

경로로 파일에서 아카이브를 열고 압축을 풉니다.`메모리 스트림`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new GzipArchive("archive.gz"))
  archive.Open().CopyTo(ms);
```

### 또한보십시오

* class [GzipArchive](../)
* 네임스페이스 [Aspose.Zip.Gzip](../../gziparchive/)
* 집회 [Aspose.Zip](../../../)


