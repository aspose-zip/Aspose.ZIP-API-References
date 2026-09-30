---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "IsoArchive 메서드. 지정된 경로에 ISO 이미지를 저장합니다."
type: docs
weight: 70
url: /ko/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

ISO 이미지를 지정된 경로에 저장합니다.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | ISO 이미지가 저장될 경로. |
| saveOptions | IsoSaveOptions | ISO 아카이브를 저장하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브가 편집 모드가 아닌 경우 발생합니다. |
| ArgumentNullException | *path*가 null인 경우 발생합니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않은 경우(예: 매핑되지 않은 드라이브에 있는 경우) 발생합니다. |
| IOException | 파일이 이미 열려 있는 경우 발생합니다. |
| UnauthorizedAccessException | 파일 *path*에 대한 접근이 거부된 경우 발생합니다. |
| PathTooLongException | 지정된 *path*가 시스템 정의 최대 길이를 초과하는 경우 발생합니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

다음 예제는 ISO 아카이브를 파일에 저장하는 방법을 보여줍니다:

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

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

ISO 이미지를 지정된 스트림에 저장합니다.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | ISO 이미지가 저장될 스트림. |
| saveOptions | IsoSaveOptions | ISO 아카이브를 저장하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브가 편집 모드가 아닌 경우 발생합니다. |
| ArgumentNullException | *stream*이 null인 경우 발생합니다. |
| ArgumentException | *stream*이 쓰기 가능하지 않을 때 발생합니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| IOException | I/O 오류가 발생했습니다. |

## 예제

다음 예제는 ISO 아카이브를 메모리 스트림에 저장하는 방법을 보여줍니다:

```csharp

 // 새 빈 ISO 아카이브 만들기
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // ISO 아카이브에 파일 추가
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // ISO 아카이브를 메모리 스트림에 저장합니다
     isoArchive.Save(memoryStream);
 }
```

### 또 보기

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


