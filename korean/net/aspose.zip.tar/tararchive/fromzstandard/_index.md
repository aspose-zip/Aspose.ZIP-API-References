---
title: "TarArchive.FromZstandard"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "TarArchive 메서드. 제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 TarArchive를 구성합니다."
type: docs
weight: 80
url: /ko/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 [`TarArchive`](../)를 구성합니다.

중요: Zstandard 아카이브는 이 메서드 내에서 완전히 추출되며, 내용이 내부에 보관됩니다. 메모리 사용량에 유의하십시오.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 소스 | 스트림 | 아카이브의 소스입니다. |

### 반환 값

[`TarArchive`](../)의 인스턴스

### 예외

| 예외 | 조건 |
| --- | --- |
| IOException | Zstandard 스트림이 손상되었거나 읽을 수 없습니다. |
| InvalidDataException | 데이터가 손상되었습니다. |
| EndOfStreamException | 예상된 바이트 수가 읽히기 전에 스트림의 끝에 도달하면 발생합니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |

### 또 보기

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 [`TarArchive`](../)를 구성합니다.

중요: Zstandard 아카이브는 이 메서드 내에서 완전히 추출되며, 내용이 내부에 보관됩니다. 메모리 사용량에 유의하십시오.

```csharp
public static TarArchive FromZstandard(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일의 경로입니다. |

### 반환 값

[`TarArchive`](../)의 인스턴스

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path*에 있는 파일이 잘못된 형식입니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| IOException | Zstandard 스트림이 손상되었거나 읽을 수 없습니다. |
| InvalidDataException | 데이터가 손상되었습니다. |
| EndOfStreamException | 예상된 바이트 수가 읽히기 전에 스트림의 끝에 도달하면 발생합니다. |

### 또 보기

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


