---
title: RarArchive.RarArchive
second_title: .NET API 참조용 Aspose.ZIP
description: RarArchive 건설자. 의 새 인스턴스를 초기화합니다.RarArchive 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.
type: docs
weight: 10
url: /ko/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`RarArchive`](../) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 아카이브 파일의 정규화된 경로 또는 상대 경로입니다. |
| loadOptions | RarArchiveLoadOptions | 기존 아카이브를 로드하는 옵션. |

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

이 생성자는 항목의 압축을 풀지 않습니다. 보다[`Open`](../../rararchiveentry/open/) 압축 해제 방법.

### 예

다음 예는 아카이브를 추출한 다음 첫 번째 항목을`메모리 스트림`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 또한보십시오

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* 네임스페이스 [Aspose.Zip.Rar](../../rararchive/)
* 집회 [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

의 새 인스턴스를 초기화합니다.[`RarArchive`](../) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | Stream | 아카이브의 소스입니다. |
| loadOptions | RarArchiveLoadOptions | 기존 아카이브를 로드하는 옵션. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *sourceStream* 찾을 수 없습니다. |
| InvalidDataException | 아카이브에 대한 잘못된 서명입니다. - 또는 - 파일이 RAR 아카이브가 아닙니다. |
| InvalidOperationException |  |

### 비고

이 생성자는 항목의 압축을 풀지 않습니다. 보다[`Open`](../../rararchiveentry/open/) 압축 해제 방법.

### 예

다음 예제는 첫 번째 항목을 해독하고 압축을 풉니다.`메모리 스트림`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### 또한보십시오

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* 네임스페이스 [Aspose.Zip.Rar](../../rararchive/)
* 집회 [Aspose.Zip](../../../)


