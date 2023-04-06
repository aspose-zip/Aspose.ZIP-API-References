---
title: TarArchive.CreateEntry
second_title: .NET API 참조용 Aspose.ZIP
description: TarArchive 방법. 아카이브 내에 단일 항목을 생성합니다.
type: docs
weight: 80
url: /ko/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| source | Stream | 항목의 입력 스트림입니다. |
| fileInfo | FileSystemInfo | 압축할 파일 또는 폴더의 메타데이터입니다. |

### 반환 값

타르 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 표준의 tar에 비해 너무 깁니다. |
| ArgumentException | 파일 이름(일부)*name*, 100개 기호를 초과합니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*fileInfo* 매개변수는 항목 이름에 영향을 주지 않습니다.

*fileInfo* 참조할 수 있습니다DirectoryInfo 항목이 디렉토리인 경우.

### 예

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### 또한보십시오

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축할 파일 또는 폴더의 메타데이터입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

### 반환 값

타르 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 표준의 tar에 비해 너무 깁니다. |
| ArgumentException | 파일 이름(일부)*name*, 100개 기호를 초과합니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*fileInfo* 매개변수는 항목 이름에 영향을 주지 않습니다.

*fileInfo* 참조할 수 있습니다DirectoryInfo 항목이 디렉토리인 경우.

파일을 즉시 열면*openImmediately*매개변수는 아카이브가 삭제될 때까지 차단됩니다.

### 예

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### 또한보십시오

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| path | String | 압축할 파일의 경로입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

### 반환 값

타르 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *path* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*path* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. - 또는 - 의 일부인 파일 이름*name*, 100개 기호를 초과합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*path* 거부되었습니다. |
| PathTooLongException | 지정된*path* , 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. - 또는 -*name* IEEE 1003.1-1998 표준의 tar에 비해 너무 깁니다. |
| NotSupportedException | 파일 위치*path* 문자열 중간에 콜론(:)을 포함합니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*path* 매개변수는 항목 이름에 영향을 주지 않습니다.

파일을 즉시 열면*openImmediately*매개변수는 아카이브가 삭제될 때까지 차단됩니다.

### 예

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### 또한보십시오

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* 네임스페이스 [Aspose.Zip.Tar](../../tararchive/)
* 집회 [Aspose.Zip](../../../)


