---
title: Archive.Save
second_title: .NET API 참조용 Aspose.ZIP
description: Archive 방법. 제공된 스트림에 아카이브를 저장합니다.
type: docs
weight: 90
url: /ko/net/aspose.zip/archive/save/
---
## Save(Stream, ArchiveSaveOptions) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream outputStream, ArchiveSaveOptions saveOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| outputStream | Stream | 대상 스트림. |
| saveOptions | ArchiveSaveOptions | 아카이브 저장 옵션. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *outputStream* 쓸 수 없습니다. |

### 비고

*outputStream*쓰기 가능해야 합니다.

### 예

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry.bin", "data.bin");
        archive.Save(zipFile);
    }
}
```

### 또한보십시오

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)

---

## Save(string, ArchiveSaveOptions) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName, ArchiveSaveOptions saveOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |
| saveOptions | ArchiveSaveOptions | 아카이브 저장 옵션. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *destinationFileName* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*destinationFileName* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*destinationFileName* 거부되었습니다. |
| PathTooLongException | 지정된*destinationFileName*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어, Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*destinationFileName* 문자열 중간에 콜론(:)을 포함합니다. |

### 비고

에서 로드된 것과 동일한 경로에 아카이브를 저장할 수 있습니다. 그러나 이 방법은 임시 파일에 복사하는 방식을 사용하기 때문에 권장되지 않습니다.

### 예

```csharp
using (var archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.zip",  new ArchiveSaveOptions() { Encoding = Encoding.ASCII });
}
```

### 또한보십시오

* class [ArchiveSaveOptions](../../../aspose.zip.saving/archivesaveoptions/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)


