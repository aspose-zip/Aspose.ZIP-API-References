---
title: "CabArchive.Save"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "CabArchive 메서드. 제공된 스트림에 아카이브를 저장합니다."
type: docs
weight: 70
url: /ko/net/aspose.zip.cab/cabarchive/save/
---
## Save(Stream, CabSaveOptions) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream outputStream, CabSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| outputStream | 스트림 | 대상 스트림. |
| saveOptions | CabSaveOptions | 아카이브 저장 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | *outputStream*은 쓰기 및 탐색이 불가능합니다. |
| ObjectDisposedException | 아카이브가 해제되었습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되었으며 저장할 수 없습니다. |

## 비고

*outputStream* must be writable.

## 예제

```csharp
using (FileStream cabFile = File.Open("archive.cab", FileMode.Create))
{
    using (var archive = new CabArchive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(cabFile);
    }
}
```

### 또 보기

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, CabSaveOptions) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName, CabSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |
| saveOptions | CabSaveOptions | 아카이브 저장 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *destinationFileName*이(가) null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *destinationFileName*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *destinationFileName* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *destinationFileName* 또는 파일 이름, 혹은 둘 다가 시스템 정의 최대 길이를 초과했습니다. 예를 들어 Windows 기반 플랫폼에서는 경로 길이가 248자 미만이어야 하고, 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *destinationFileName* 위치의 파일 이름에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 열려 있습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

아카이브를 로드된 동일한 경로에 저장할 수 있습니다. 그러나 이 방법은 임시 파일에 복사하는 방식을 사용하므로 권장되지 않습니다.

## 예제

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### 또 보기

* class [CabSaveOptions](../../cabsaveoptions/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


