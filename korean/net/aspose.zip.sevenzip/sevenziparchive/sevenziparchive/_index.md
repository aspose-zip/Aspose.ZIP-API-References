---
title: SevenZipArchive.SevenZipArchive
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipArchive 건설자. 의 새 인스턴스를 초기화합니다.SevenZipArchive 항목에 대한 선택적 설정이 있는 클래스.
type: docs
weight: 10
url: /ko/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

의 새 인스턴스를 초기화합니다.[`SevenZipArchive`](../) 항목에 대한 선택적 설정이 있는 클래스.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | 새로 추가된 파일에 사용되는 압축 및 암호화 설정[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. 지정하지 않으면 암호화 없는 LZMA 압축이 사용됩니다. |

### 예

다음 예제는 기본 설정으로 단일 파일을 압축하는 방법을 보여줍니다: 암호화 없이 LZMA 압축.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### 또한보십시오

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`SevenZipArchive`](../) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | Stream | 아카이브의 소스입니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *sourceStream* 찾을 수 없습니다. |
| ArgumentNullException | *sourceStream* null입니다. |
| NotImplementedException | 아카이브에는 둘 이상의 코더가 포함되어 있습니다. 이제 LZMA 압축만 지원됩니다. |

### 비고

이 생성자는 항목의 압축을 풀지 않습니다. 보다[`ExtractToDirectory`](../extracttodirectory/) 압축 해제 방법.

### 예

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 또한보십시오

* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

의 새 인스턴스를 초기화합니다.[`SevenZipArchive`](../) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.

```csharp
public SevenZipArchive(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 아카이브 파일의 정규화된 경로 또는 상대 경로입니다. |

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

이 생성자는 항목의 압축을 풀지 않습니다. 보다[`ExtractToDirectory`](../extracttodirectory/) 압축 해제 방법.

### 예

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### 또한보십시오

* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)


