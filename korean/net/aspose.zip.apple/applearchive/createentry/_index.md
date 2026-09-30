---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AppleArchive 메서드. 아카이브 내에 단일 항목을 생성합니다"
type: docs
weight: 60
url: /ko/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| 경로 | String | 압축할 파일의 경로입니다. |
| openImmediately | Boolean | 파일을 즉시 열 경우 True, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

### 반환 값

Apple Archive 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었습니다. |
| ArgumentException | *name*이 비어 있습니다. |
| ArgumentNullException | *path*는 `null`입니다. |

### 또 보기

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| 소스 | 스트림 | 항목에 대한 입력 스트림입니다. |

### 반환 값

Apple Archive 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었습니다. |
| ArgumentException | *name*이 비어 있습니다. |
| ArgumentNullException | *source*은 `null`입니다. |

### 또 보기

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축될 파일의 메타데이터입니다. |
| openImmediately | Boolean | 파일을 즉시 열 경우 True, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

### 반환 값

Apple Archive 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었습니다. |
| ArgumentException | *name*이 비어 있습니다. |
| ArgumentNullException | *fileInfo*은 `null`입니다. |

### 또 보기

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


