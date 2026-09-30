---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "AlzArchive 생성자. 스트림에서 AlzArchive 클래스의 새 인스턴스를 초기화합니다"
type: docs
weight: 10
url: /ko/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

스트림에서 [`AlzArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 스트림 | 스트림 | ALZ 아카이브 스트림입니다. 스트림은 읽기 및 탐색을 지원해야 합니다. |
| loadOptions | AlzArchiveLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | 스트림이 null입니다. |

### 또 보기

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

파일 경로에서 [`AlzArchive`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| filePath | String | ALZ 아카이브 파일의 경로입니다. |
| loadOptions | AlzArchiveLoadOptions | 기존 아카이브를 로드하기 위한 옵션. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | filePath이 null입니다. |
| FileNotFoundException | 파일이 존재하지 않습니다. |

### 또 보기

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


