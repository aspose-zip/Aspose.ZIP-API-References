---
title: "XarArchive.Save"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarArchive 메서드. 제공된 대상 파일에 아카이브를 저장합니다."
type: docs
weight: 80
url: /ko/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |
| saveOptions | XarSaveOptions | xar 아카이브를 저장하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *destinationFileName*이(가) null입니다. |
| InvalidOperationException | xar 아카이브를 수정할 수 없습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| IOException | 파일을 여는 중 I/O 오류가 발생했습니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 둘 다가 시스템에서 정의한 최대 길이를 초과합니다. |
| UnauthorizedAccessException | *destinationFileName*이 읽기 전용 파일을 지정했습니다. -또는- *destinationFileName*이 디렉터리를 지정했습니다. -또는- 호출자가 필요한 권한이 없습니다. |

### 또 보기

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| output | 스트림 | 대상 스트림. |
| saveOptions | XarSaveOptions | xar 아카이브를 저장하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *output*이 null입니다. |
| ArgumentException | *output*은 쓰기/읽기가 불가능하거나 탐색할 수 없습니다. |
| InvalidOperationException | xar 아카이브를 수정할 수 없습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

### 또 보기

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


