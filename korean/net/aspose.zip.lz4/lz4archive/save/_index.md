---
title: "Lz4Archive.Save"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "Lz4Archive 메서드. 제공된 스트림에 lz4 아카이브를 저장합니다."
type: docs
weight: 60
url: /ko/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

제공된 스트림에 lz4 아카이브를 저장합니다.

```csharp
public void Save(Stream output)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| output | 스트림 | 대상 스트림. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *output*이 null입니다. |
| ArgumentException | *output*은(는) 쓰기 가능하지 않습니다. |
| InvalidOperationException | 아카이브가 추출 준비되었습니다. - 또는 - 소스가 제공되지 않았습니다. |
| OperationCanceledException | .NET Framework 4.0 이상에서: 제공된 취소 토큰을 통해 압축이 취소될 때 발생합니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

*output* must be seekable.

## 예제

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### 또 보기

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

제공된 대상 파일에 lz4 아카이브를 저장합니다.

```csharp
public void Save(FileInfo destination)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 대상 | FileInfo | FileInfo, 대상 스트림으로 열립니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| SecurityException | 호출자에게 *destination*을 열 권한이 없습니다. |
| ArgumentException | 파일 경로가 비어 있거나 공백만 포함합니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| UnauthorizedAccessException | 파일 경로가 읽기 전용이거나 디렉터리입니다. |
| ArgumentNullException | *destination*이 null입니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되었습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### 또 보기

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *destinationFileName*이(가) null입니다. |
| SecurityException | 호출자에게 접근에 필요한 권한이 없습니다. |
| ArgumentException | *destinationFileName*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *destinationFileName* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *destinationFileName* 또는 파일 이름, 혹은 둘 다가 시스템 정의 최대 길이를 초과했습니다. 예를 들어 Windows 기반 플랫폼에서는 경로 길이가 248자 미만이어야 하고, 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *destinationFileName* 위치의 파일 이름에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되었습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다(예: 매핑되지 않은 드라이브에 있는 경우). |
| FileNotFoundException | *destinationFileName*에 지정된 파일을 찾을 수 없습니다. |
| IOException | 파일을 여는 중 I/O 오류가 발생했습니다. |

## 예제

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### 또 보기

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


