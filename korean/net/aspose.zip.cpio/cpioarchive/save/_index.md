---
title: CpioArchive.Save
second_title: .NET API 참조용 Aspose.ZIP
description: CpioArchive 방법. 제공된 대상 파일에 아카이브를 저장합니다.
type: docs
weight: 80
url: /ko/net/aspose.zip.cpio/cpioarchive/save/
---
## Save(string, CpioFormat) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *destinationFileName* 길이가 0인 문자열이거나, 공백만 포함하거나, System.IO.Path.InvalidPathChars에서 정의한 잘못된 문자를 하나 이상 포함합니다. |
| ArgumentNullException | *destinationFileName* null입니다. |
| PathTooLongException | 지정된*destinationFileName*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| DirectoryNotFoundException | 지정된*destinationFileName* 유효하지 않습니다(예: 매핑되지 않은 드라이브에 있음). |
| IOException | 파일을 여는 동안 I/O 오류가 발생했습니다. |
| UnauthorizedAccessException | *destinationFileName* 읽기 전용이고 액세스 권한이 읽기 전용이 아닌 파일을 지정했습니다. 또는 경로가 디렉터리를 지정했습니다. 또는 호출자에게 필요한 권한이 없습니다. |
| NotSupportedException | *destinationFileName* 잘못된 형식입니다. |

### 비고

에서 로드된 것과 동일한 경로에 아카이브를 저장할 수 있습니다. 그러나 이 방법은 임시 파일에 복사하는 방식을 사용하기 때문에 권장되지 않습니다.

### 예

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("archive.cpio");
}       
```

### 또한보십시오

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)

---

## Save(Stream, CpioFormat) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| output | Stream | 대상 스트림. |
| cpioFormat | CpioFormat | cpio 헤더 형식을 정의합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *output* null입니다. |
| ArgumentException | *output* 쓸 수 없습니다. - 또는 -*output* 우리가 추출한 것과 동일한 스트림입니다. - 또는 - 아카이브를 저장할 수 없습니다.*cpioFormat* 형식 제한 때문입니다. |

### 비고

*output*쓰기 가능해야 합니다.

### 예

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry1", "data.bin");        
        archive.Save(cpioFile);
    }
}       
```

### 또한보십시오

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)


