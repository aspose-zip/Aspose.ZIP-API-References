---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP에 대한 .NET API 참조"
description: "ArjEntryPlain 메서드. 제공된 경로에 따라 항목을 파일 시스템에 추출합니다"
type: docs
weight: 40
url: /ko/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다.

```csharp
public FileInfo Extract(string path)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 경로 | String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

### 반환 값

조합된 파일의 파일 정보입니다.

### 예외

| 예외 | 조건 |
| --- | --- |
| ArgumentNullException | *path*가 null이거나 비어 있습니다. |
| ObjectDisposedException | 아카이브가 해제된 경우 발생합니다. |
| FileNotFoundException | 파일을 찾을 수 없습니다. |
| InvalidDataException | 헤더 또는 데이터의 체크섬이 일치하지 않습니다. - 또는 - 아카이브가 손상되었습니다. |
| PathTooLongException | 지정된 경로, 파일 이름 또는 둘 다가 시스템에서 정의한 최대 길이를 초과합니다. |
| NotImplementedException | 항목이 메서드 4로 압축되었습니다. |

## 예제

rar 아카이브의 두 항목을 추출합니다.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### 또 보기

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

ARJ 아카이브 항목을 파일로 추출합니다.

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
| ObjectDisposedException | 아카이브가 해제된 경우 발생합니다. |
| InvalidDataException | 헤더 또는 데이터의 체크섬이 일치하지 않습니다. - 또는 - 아카이브가 손상되었습니다. |
| NotImplementedException | 항목이 메서드 4로 압축되었습니다. |

## 예제

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### 또 보기

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
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
| InvalidDataException | 헤더 또는 데이터의 체크섬이 일치하지 않습니다. - 또는 - 아카이브가 손상되었습니다. |
| NotImplementedException | 항목이 메서드 4로 압축되었습니다. |
| OperationCanceledException | .NET Framework 4.0 이상: 제공된 취소 토큰을 통해 추출이 취소될 때 발생합니다. |
| ObjectDisposedException | 아카이브가 해제된 경우 발생합니다. |

### 또 보기

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


