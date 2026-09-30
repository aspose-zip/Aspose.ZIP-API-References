---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "XarArchive 메서드. 아카이브 내에 단일 항목을 생성합니다"
type: docs
weight: 40
url: /ko/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축될 파일 또는 폴더의 메타데이터입니다. |
| openImmediately | Boolean | 파일을 즉시 열 경우 True, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |
| compressionSettings | XarCompressionSettings | 추가된 [`XarEntry`](../../xarentry/) 항목에 사용되는 압축 설정입니다. |

### 반환 값

Xar 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *name*이 null입니다. |
| ArgumentException | *name*이 비어 있습니다. |
| ArgumentNullException | *fileInfo*가 null입니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

*openImmediately* 매개변수로 파일을 즉시 열면 아카이브가 해제될 때까지 파일이 차단됩니다.

## 예제

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### 또 보기

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| sourcePath | String | 압축될 파일의 경로. |
| openImmediately | Boolean | 파일을 즉시 열 경우 True, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |
| compressionSettings | XarCompressionSettings | 추가된 [`XarEntry`](../../xarentry/) 항목에 사용되는 압축 설정입니다. |

### 반환 값

Xar 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *sourcePath*은 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *sourcePath*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. - 또는 - 파일 이름이 *name*의 일부로서 100자를 초과합니다. |
| UnauthorizedAccessException | 파일 *sourcePath*에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *sourcePath*, 파일 이름 또는 두 개 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로 길이가 248자 미만이어야 하고, 파일 이름은 260자 미만이어야 합니다. - 또는 - *name*이 xar에 대해 너무 깁니다. |
| NotSupportedException | 파일 *sourcePath*에 콜론 (:)이 문자열 중간에 포함되어 있습니다. |
| InvalidOperationException | xar 아카이브를 수정할 수 없습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 비고

엔트리 이름은 *name* 매개변수 내에서만 설정됩니다. *sourcePath* 매개변수에 제공된 파일 이름은 엔트리 이름에 영향을 주지 않습니다.

*openImmediately* 매개변수로 파일을 즉시 열면 아카이브가 해제될 때까지 파일이 차단됩니다.

## 예제

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### 또 보기

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| 소스 | 스트림 | 항목에 대한 입력 스트림입니다. |
| compressionSettings | XarCompressionSettings | 추가된 [`XarEntry`](../../xarentry/) 항목에 사용되는 압축 설정입니다. |

### 반환 값

Xar 항목 인스턴스입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *name*이 null입니다. |
| ArgumentNullException | *source*이 null입니다. |
| ArgumentException | *name*이 비어 있습니다. |
| InvalidOperationException | xar 아카이브를 수정할 수 없습니다. |
| ObjectDisposedException | 아카이브가 해제되었으며 사용할 수 없습니다. |

## 예제

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### 또 보기

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


