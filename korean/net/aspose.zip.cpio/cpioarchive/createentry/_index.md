---
title: CpioArchive.CreateEntry
second_title: .NET API 참조용 Aspose.ZIP
description: CpioArchive 방법. 아카이브 내에 단일 항목을 생성합니다.
type: docs
weight: 40
url: /ko/net/aspose.zip.cpio/cpioarchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CpioEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축할 파일 또는 폴더의 메타데이터입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

### 반환 값

Cpio 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *name* null입니다. |
| ArgumentException | *name* 비었다. |
| ArgumentNullException | *fileInfo* null입니다. |

### 비고

파일을 즉시 열면*openImmediately*매개변수는 아카이브가 삭제될 때까지 차단됩니다.

### 예

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new CpioArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.cpio");
}
```

### 또한보십시오

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CpioEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| sourcePath | String | 압축할 파일의 경로입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

### 반환 값

Cpio 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *sourcePath* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*sourcePath* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. - 또는 - 의 일부인 파일 이름*name*, 100개 기호를 초과합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*sourcePath* 거부되었습니다. |
| PathTooLongException | 지정된*sourcePath* , 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. - 또는 -*name* cpio에 대해 너무 깁니다. |
| NotSupportedException | 파일 위치*sourcePath* 문자열 중간에 콜론(:)을 포함합니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*sourcePath* 매개변수는 항목 이름에 영향을 주지 않습니다.

파일을 즉시 열면*openImmediately*매개변수는 아카이브가 삭제될 때까지 차단됩니다.

### 예

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### 또한보십시오

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CpioEntry CreateEntry(string name, Stream source)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| source | Stream | 항목의 입력 스트림입니다. |

### 반환 값

Cpio 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *name* null입니다. |
| ArgumentNullException | *source* null입니다. |
| ArgumentException | *name* 비었다. |

### 예

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.cpio");
}
```

### 또한보십시오

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* 네임스페이스 [Aspose.Zip.Cpio](../../cpioarchive/)
* 집회 [Aspose.Zip](../../../)


