---
title: "UueArchive.SetSource"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "UueArchive 메서드. 아카이브 내에 인코딩될 내용을 설정합니다"
type: docs
weight: 80
url: /ko/net/aspose.zip.uue/uuearchive/setsource/
---
## SetSource(Stream) {#setsource_1}

아카이브 내에서 인코딩될 내용을 설정합니다.

```csharp
public void SetSource(Stream source)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 소스 | 스트림 | 아카이브의 입력 스트림입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.uue");
}
```

### 또 보기

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

아카이브 내에서 압축될 내용을 설정합니다.

```csharp
public void SetSource(FileInfo fileInfo)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileInfo | FileInfo | 압축될 파일에 대한 참조입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.uue");
}
```

### 또 보기

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

아카이브 내에서 인코딩될 내용을 설정합니다.

```csharp
public void SetSource(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 인코딩될 파일의 경로입니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |

## 예제

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


