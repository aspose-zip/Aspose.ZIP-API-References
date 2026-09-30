---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AppleArchive 생성자. 구성된 엔트리에 사용되는 설정으로 AppleArchive 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

구성된 엔트리에 사용되는 설정으로 [`AppleArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | 새 Apple Archive를 구성할 때 사용되는 설정. |

### 또 보기

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

[`AppleArchive`](../) 클래스의 새 인스턴스를 초기화하고, 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| sourceStream | 스트림 | 아카이브의 소스입니다. |
| loadOptions | AppleArchiveLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *sourceStream*이 null입니다. |
| ArgumentException | *sourceStream*은 검색 가능하지 않습니다. |
| InvalidDataException | *sourceStream* 은(는) 유효한 Apple Archive가 아닙니다. |
| EndOfStreamException | 아카이브 엔트리를 구문 분석하는 중에 스트림이 예기치 않게 종료되었습니다. |

## 비고

이 생성자는 어떤 엔트리도 압축을 해제하지 않습니다. 압축 해제를 위해 [`ExtractToDirectory`](../extracttodirectory/) 및 [`Open`](../../applearchiveentry/open/) 메서드를 참조하십시오.

### 또 보기

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

[`AppleArchive`](../) 클래스의 새 인스턴스를 초기화하고, 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 아카이브 파일에 대한 전체 경로나 상대 경로입니다. |
| loadOptions | AppleArchiveLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| InvalidDataException | *path* 은(는) 유효한 Apple Archive가 아닙니다. |
| EndOfStreamException | 아카이브 엔트리를 구문 분석하는 중에 스트림이 예기치 않게 종료되었습니다. |

## 비고

이 생성자는 어떤 엔트리도 압축을 해제하지 않습니다. 압축 해제를 위해 [`ExtractToDirectory`](../extracttodirectory/) 및 [`Open`](../../applearchiveentry/open/) 메서드를 참조하십시오.

### 또 보기

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


