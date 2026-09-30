---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoArchive 생성자. IsoArchive 클래스의 새 인스턴스를 초기화하고 새 파일 및 디렉터리를 추가하기 위한 빈 ISO 아카이브를 생성합니다."
type: docs
weight: 10
url: /ko/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

[`IsoArchive`](../) 클래스의 새 인스턴스를 초기화하고 새 파일 및 디렉터리를 추가하기 위한 빈 ISO 아카이브를 생성합니다.

```csharp
public IsoArchive()
```

## 예제

다음 예제에서는 새 빈 ISO 아카이브를 만들고 파일을 추가하는 방법을 보여줍니다:

```csharp
// 새 빈 ISO 아카이브 만들기
using(IsoArchive isoArchive = new IsoArchive())
{
    // ISO 아카이브에 파일 추가
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO 아카이브를 파일에 저장
    isoArchive.Save("new_archive.iso");
}
```

### 또 보기

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

[`IsoArchive`](../) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceStream | 스트림 | 아카이브의 소스입니다. 검색 가능해야 합니다. |
| loadOptions | IsoLoadOptions | 아카이브를 로드할 옵션입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *sourceStream*이 null입니다. |
| ArgumentException | *sourceStream*은 검색 가능하지 않습니다. |
| InvalidDataException | *sourceStream*은 유효한 ISO 아카이브가 아닙니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| EndOfStreamException | 스트림의 끝에 예기치 않게 도달했을 때 발생합니다. |
| IOException | I/O 오류가 발생했습니다. |
| NotSupportedException | 스트림이 읽기를 지원하지 않습니다. |

## 비고

이 생성자는 항목을 풀어내지 않습니다.

## 예제

다음 예제에서는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 또 보기

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

[`IsoArchive`](../) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일의 경로입니다. |
| loadOptions | IsoLoadOptions | 아카이브를 로드할 옵션입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |
| EndOfStreamException | 파일이 너무 짧습니다. |
| InvalidDataException | 데이터가 유효하지 않거나 손상된 경우에 발생합니다. |

## 비고

이 생성자는 항목을 풀어내지 않습니다.

## 예제

다음 예제에서는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### 또 보기

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


