---
title: "UueArchive.Save"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "UueArchive 메서드. 제공된 스트림에 아카이브를 저장합니다."
type: docs
weight: 70
url: /ko/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| outputStream | 스트림 | 대상 스트림. |
| saveOptions | UueSaveOptions | 아카이브 저장 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| InvalidOperationException | 아카이브할 데이터 소스가 제공되지 않았습니다. |
| ArgumentException | *outputStream*은(는) 쓰기 가능하지 않습니다. |
| UnauthorizedAccessException | 파일 소스가 읽기 전용이거나 디렉터리입니다. |
| DirectoryNotFoundException | 지정된 파일 소스 경로가 잘못되었습니다. 예를 들어 매핑되지 않은 드라이브에 있을 수 있습니다. |
| IOException | 파일 소스가 이미 열려 있습니다. |

## 비고

*outputStream* must be writable.

## 예제

압축된 데이터를 http 응답 스트림에 씁니다.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 또 보기

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |
| saveOptions | UueSaveOptions | 아카이브 저장 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| ArgumentNullException | *destinationFileName*이(가) null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *destinationFileName*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *destinationFileName* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *destinationFileName* 또는 파일 이름, 혹은 둘 다가 시스템 정의 최대 길이를 초과했습니다. 예를 들어 Windows 기반 플랫폼에서는 경로 길이가 248자 미만이어야 하고, 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *destinationFileName* 위치의 파일 이름에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| InvalidOperationException | 아카이브할 데이터 소스가 제공되지 않았습니다. |

## 예제

인코딩된 데이터를 파일에 씁니다.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### 또 보기

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


