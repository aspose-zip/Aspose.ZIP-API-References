---
title: Bzip2Archive.Save
second_title: .NET API 참조용 Aspose.ZIP
description: Bzip2Archive 방법. 제공된 스트림에 아카이브를 저장합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| outputStream | Stream | 대상 스트림. |
| saveOptions | Bzip2SaveOptions | bzip2 아카이브 저장 옵션. 지정하지 않으면 900Kb 블록 크기가 사용됩니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| InvalidOperationException | 보관할 데이터 소스가 제공되지 않았습니다. |
| ArgumentException | *outputStream* 쓸 수 없습니다. |
| UnauthorizedAccessException | 파일 소스가 읽기 전용이거나 디렉토리입니다. |
| DirectoryNotFoundException | 매핑되지 않은 드라이브에 있는 것과 같이 지정된 파일 소스 경로가 잘못되었습니다. |
| IOException | 파일 소스가 이미 열려 있습니다. |

### 비고

*outputStream*쓰기 가능해야 합니다.

### 예

압축된 데이터를 http 응답 스트림에 씁니다.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### 또한보십시오

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* 네임스페이스 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 집회 [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성할 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 덮어씁니다. |
| saveOptions | Bzip2SaveOptions | bzip2 아카이브 저장 옵션. 지정하지 않으면 900Kb 블록 크기가 사용됩니다. |

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *destinationFileName* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*destinationFileName* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*destinationFileName* 거부되었습니다. |
| PathTooLongException | 지정된*destinationFileName*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*destinationFileName* 문자열 중간에 콜론(:)을 포함합니다. |

### 예

압축된 데이터를 파일에 기록합니다.

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### 또한보십시오

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* 네임스페이스 [Aspose.Zip.Bzip2](../../bzip2archive/)
* 집회 [Aspose.Zip](../../../)


