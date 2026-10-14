---
title: "UueArchive.UueArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "UueArchive 생성자. 인코딩을 위해 준비된 UueArchive 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

인코딩을 위해 준비된 [`UueArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public UueArchive()
```

## 예제

다음 예제는 파일을 uuencode 하는 방법을 보여줍니다.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### 또 보기

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

디코딩을 위해 준비된 [`UueArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public UueArchive(Stream sourceStream)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceStream | 스트림 | 아카이브의 소스입니다. |

## 비고

이 생성자는 디코딩하지 않습니다. 압축 해제를 위해 [`Open`](../open/) 메서드를 참조하십시오.

## 예제

스트림에서 아카이브를 열고 `MemoryStream`에 추출합니다.

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### 또 보기

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

[`UueArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public UueArchive(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일의 경로입니다. |

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
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| IOException | 파일이 이미 열려 있습니다. |

## 비고

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [`Open`](../open/) 메서드를 참조하십시오.

## 예제

파일 경로에서 아카이브를 열고 `MemoryStream`으로 디코드합니다

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### 또 보기

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


