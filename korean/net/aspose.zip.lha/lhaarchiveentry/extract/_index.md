---
title: "LhaArchiveEntry.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "LhaArchiveEntry 메서드. 경로에 따라 Lha 아카이브 항목을 파일 시스템에 추출합니다."
type: docs
weight: 60
url: /ko/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Lha 아카이브 항목을 경로를 통해 파일 시스템에 추출합니다.

```csharp
public FileSystemInfo Extract(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 압축 해제된 데이터를 저장할 파일 경로. |

### 반환 값

추출된 데이터를 포함하는 FileSystemInfoInstance.

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브 헤더와 서비스 정보가 읽히지 않았습니다. |
| ArgumentNullException | *path*이 null입니다. |
| SecurityException | 호출자는 접근에 필요한 권한이 없습니다. |
| ArgumentException | *path*이 비어 있거나, 공백만 포함하거나, 잘못된 문자를 포함하고 있습니다. |
| UnauthorizedAccessException | *path* 파일에 대한 접근이 거부되었습니다. |
| PathTooLongException | 지정된 *path* 또는 파일 이름, 혹은 둘 모두가 시스템에서 정의한 최대 길이를 초과했습니다. 예를 들어, Windows 기반 플랫폼에서는 경로가 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | *path* 위치의 파일에 문자열 중간에 콜론 (:)이 포함되어 있습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| InvalidDataException | 데이터가 유효하지 않거나 손상된 경우에 발생합니다. |

## 예제

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### 또 보기

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

제공된 스트림으로 항목을 추출합니다.

```csharp
public void Extract(Stream destination)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 대상 | 스트림 | 대상 스트림. 쓰기 가능해야 합니다. |

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentException | *destination* 은(는) 쓰기를 지원하지 않습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |
| InvalidDataException | 데이터가 유효하지 않거나 손상된 경우에 발생합니다. |

## 비고

디렉터리 항목에 대해서는 아무 작업도 수행하지 않습니다.

### 또 보기

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Lha 아카이브 항목을 파일로 추출합니다.

```csharp
public void Extract(FileInfo fileInfo)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| fileInfo | FileInfo | 압축 해제된 데이터를 저장하기 위한 FileInfo. |

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 아카이브 헤더와 서비스 정보가 읽히지 않았습니다. |
| SecurityException | 호출자에게 *fileInfo*를 열 권한이 없습니다. |
| ArgumentException | 파일 경로가 비어 있거나 공백만 포함합니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| UnauthorizedAccessException | 파일 경로가 읽기 전용이거나 디렉터리입니다. |
| ArgumentNullException | *fileInfo*가 null입니다. |
| DirectoryNotFoundException | 지정된 경로가 유효하지 않습니다. 예를 들어, 매핑되지 않은 드라이브에 있을 경우입니다. |
| IOException | 파일이 이미 열려 있습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 소스 스트림이 해제된 경우 발생합니다. |

## 비고

디렉터리 항목에 대해서는 아무 작업도 수행하지 않습니다.

## 예제

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### 또 보기

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


