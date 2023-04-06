---
title: CabArchive.CabArchive
second_title: .NET API 참조용 Aspose.ZIP
description: CabArchive 건설자. 의 새 인스턴스를 초기화합니다.CabArchive 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.
type: docs
weight: 10
url: /ko/net/aspose.zip.cab/cabarchive/cabarchive/
---
## CabArchive(Stream) {#constructor}

의 새 인스턴스를 초기화합니다.[`CabArchive`](../) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.

```csharp
public CabArchive(Stream sourceStream)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | Stream | 아카이브의 소스입니다. 검색 가능해야 합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *sourceStream* null입니다. |
| ArgumentException | *sourceStream* 찾을 수 없습니다. |
| InvalidDataException | *sourceStream* 유효한 택시 아카이브가 아닙니다. |

### 비고

이 생성자는 항목의 압축을 풀지 않습니다. 보다[`Open`](../../cabentry/open/)포장 풀기 방법.

### 예

다음 예에서는 모든 항목을 디렉토리로 추출하는 방법을 보여줍니다.

```csharp
using (var archive = new CabArchive(File.OpenRead("archive.cab")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 또한보십시오

* class [CabArchive](../)
* 네임스페이스 [Aspose.Zip.Cab](../../cabarchive/)
* 집회 [Aspose.Zip](../../../)

---

## CabArchive(string) {#constructor_1}

의 새 인스턴스를 초기화합니다.[`CabArchive`](../) 클래스 및 작성 항목 목록은 아카이브에서 추출할 수 있습니다.

```csharp
public CabArchive(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 아카이브 파일의 경로입니다. |

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

이 생성자는 항목의 압축을 풀지 않습니다. 보다[`Open`](../../cabentry/open/)포장 풀기 방법.

### 예

다음 예에서는 모든 항목을 디렉토리로 추출하는 방법을 보여줍니다.

```csharp
using (var archive = new CabArchive("archive.cab")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### 또한보십시오

* class [CabArchive](../)
* 네임스페이스 [Aspose.Zip.Cab](../../cabarchive/)
* 집회 [Aspose.Zip](../../../)


