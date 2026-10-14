---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "CabArchive 메서드. 아카이브 내에 단일 항목을 생성합니다."
type: docs
weight: 40
url: /ko/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| 경로 | String | 압축될 새 파일의 전체 지정 이름 또는 상대 파일 이름. |
| newEntrySettings | CabEntrySettings | 추가된 [`CabEntry`](../../cabentry/) 항목에 사용되는 압축 및 암호화 설정. |

### 반환 값

Cab 항목 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되어 있어 항목을 추가할 수 없습니다. |

## 비고

항목 이름은 *name* 매개변수 내에서만 설정됩니다. *path* 매개변수에 제공된 파일 이름은 항목 이름에 영향을 주지 않습니다.

## 예제

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### 또 보기

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| 소스 | 스트림 | 항목에 대한 입력 스트림입니다. |
| newEntrySettings | CabEntrySettings | 추가된 [`CabEntry`](../../cabentry/) 항목에 사용되는 압축 및 암호화 설정. |

### 반환 값

Cab 항목 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되어 있어 항목을 추가할 수 없습니다. |
| ArgumentNullException | *name*이 null입니다. |

## 예제

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### 또 보기

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축될 파일의 메타데이터입니다. |
| newEntrySettings | CabEntrySettings | 추가된 [`CabEntry`](../../cabentry/) 항목에 사용되는 압축 및 암호화 설정. |

### 반환 값

CAB 항목 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo*은 읽기 전용이거나 디렉터리입니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |
| FileNotFoundException | *fileInfo*은 찾을 수 없는 파일을 나타냅니다. |
| SecurityException | 호출자는 *fileInfo*에 접근할 권한이 없습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| InvalidOperationException | 아카이브가 추출을 위해 준비되어 있어 항목을 추가할 수 없습니다. |
| ArgumentNullException | *name*이 null입니다. |

## 비고

항목 이름은 *name* 매개변수 내에서만 설정됩니다. *fileInfo* 매개변수에 제공된 파일 이름은 항목 이름에 영향을 주지 않습니다.

## 예제

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### 또 보기

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| streamProvider | Func`1 | 항목에 대한 입력 스트림을 제공하는 메서드. |
| newEntrySettings | CabEntrySettings | 추가된 [`CabEntry`](../../cabentry/) 항목에 사용되는 압축 및 암호화 설정. |

### 반환 값

CAB 항목 인스턴스.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브가 압축 해제를 위해 인스턴스화되었습니다. - 또는 - 파일 수가 제한에 도달했습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |
| ArgumentException | *name*은 null이거나 비어 있습니다. |

## 예제

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### 또 보기

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


