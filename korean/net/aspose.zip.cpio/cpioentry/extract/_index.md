---
title: CpioEntry.Extract
second_title: .NET API 참조용 Aspose.ZIP
description: CpioEntry 방법. 제공된 경로로 항목을 파일 시스템으로 추출합니다.
type: docs
weight: 60
url: /ko/net/aspose.zip.cpio/cpioentry/extract/
---
## Extract(string) {#extract}

제공된 경로로 항목을 파일 시스템으로 추출합니다.

```csharp
public FileSystemInfo Extract(string path)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| path | String | 대상 파일의 경로입니다. 파일이 이미 있으면 덮어씁니다. |

### 반환 값

구성된 파일의 파일 정보입니다.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *path* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*path* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*path* 거부되었습니다. |
| PathTooLongException | 지정된*path*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*path* 문자열 중간에 콜론(:)을 포함합니다. |

### 예

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    archive.Entries[0].Extract("data.bin");
}
```

### 또한보십시오

* class [CpioEntry](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioentry/)
* 집회 [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

제공된 스트림에 항목을 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destination | Stream | 대상 스트림. 쓰기 가능해야 합니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentException | *destination* 쓰기를 지원하지 않습니다. |

### 예

cpio 아카이브 항목을 추출합니다.

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    archive.Entries[0].Extract(httpResponseStream);
}
```

### 또한보십시오

* class [CpioEntry](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioentry/)
* 집회 [Aspose.Zip](../../../)


