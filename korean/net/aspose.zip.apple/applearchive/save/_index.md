---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AppleArchive 메서드. 제공된 스트림에 아카이브를 저장합니다."
type: docs
weight: 90
url: /ko/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

제공된 스트림에 아카이브를 저장합니다.

```csharp
public void Save(Stream output)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| output | 스트림 | 대상 스트림. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었습니다. |
| ArgumentNullException | *output* 은 `null` 입니다. |
| ArgumentException | *output*은(는) 쓰기 가능하지 않습니다. |
| ArgumentOutOfRangeException | 구성된 LZ4 또는 Zlib 블록 크기가 양수가 아닙니다. |
| NotSupportedException | 압축 설정이 없거나 지원되지 않으며, 직접 구성은 탐색할 수 없는 스트림을 사용하거나, 엔트리/아카이브 크기가 현재 Apple Archive 제한을 초과합니다. |

## 비고

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### 또 보기

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

제공된 대상 파일에 아카이브를 저장합니다.

```csharp
public void Save(string destinationFileName)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| destinationFileName | String | 생성될 아카이브의 경로. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었습니다. |
| ArgumentException | *destinationFileName* 은(는) 올바르지 않습니다. |
| ArgumentNullException | *destinationFileName* 은 `null` 입니다. |
| ArgumentOutOfRangeException | 구성된 LZ4 또는 Zlib 블록 크기가 양수가 아닙니다. |
| NotSupportedException | 압축 설정이 없거나 지원되지 않으며, 직접 구성은 탐색할 수 없는 스트림을 사용하거나, 엔트리/아카이브 크기가 현재 Apple Archive 제한을 초과합니다. |

### 또 보기

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


