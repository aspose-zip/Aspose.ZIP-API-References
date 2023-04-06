---
title: Archive.CreateEntry
second_title: .NET API 참조용 Aspose.ZIP
description: Archive 방법. 아카이브 내에 단일 항목을 생성합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip/archive/createentry/
---
## CreateEntry(string, string, bool, ArchiveEntrySettings) {#createentry_3}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public ArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| path | String | 새 파일의 정규화된 이름 또는 압축할 상대 파일 이름입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |
| newEntrySettings | ArchiveEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`ArchiveEntry`](../../archiveentry/) 안건. |

### 반환 값

Zip 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| ArgumentNullException | *path* null입니다. |
| SecurityException | 호출자에게 액세스에 필요한 권한이 없습니다. |
| ArgumentException | 그만큼*path* 비어 있거나 공백만 포함하거나 잘못된 문자를 포함합니다. |
| UnauthorizedAccessException | 파일에 대한 액세스*path* 거부되었습니다. |
| PathTooLongException | 지정된*path*, 파일 이름 또는 둘 다 시스템 정의 최대 길이를 초과합니다. 예를 들어 Windows 기반 플랫폼에서 경로는 248자 미만이어야 하고 파일 이름은 260자 미만이어야 합니다. |
| NotSupportedException | 파일 위치*path* 문자열 중간에 콜론(:)을 포함합니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*path* 매개변수는 항목 이름에 영향을 주지 않습니다.

파일을 즉시 열면*openImmediately* 아카이브가 저장될 때까지 매개변수가 차단됩니다.

### 예

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### 또한보십시오

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| source | Stream | 항목의 입력 스트림입니다. |
| newEntrySettings | ArchiveEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`ArchiveEntry`](../../archiveentry/) 안건. |

### 반환 값

Zip 항목 인스턴스.

### 예

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.zip");
}
```

### 또한보십시오

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool, ArchiveEntrySettings) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public ArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    ArchiveEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축할 파일의 메타데이터입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |
| newEntrySettings | ArchiveEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`ArchiveEntry`](../../archiveentry/) 안건. |

### 반환 값

Zip 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* 읽기 전용이거나 디렉토리입니다. |
| DirectoryNotFoundException | 매핑되지 않은 드라이브에 있는 것과 같이 지정된 경로가 잘못되었습니다. |
| IOException | 파일이 이미 열려 있습니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*fileInfo* 매개변수는 항목 이름에 영향을 주지 않습니다.

파일을 즉시 열면*openImmediately* 아카이브가 저장될 때까지 매개변수가 차단됩니다.

### 예

각각 다른 암호화 방법과 비밀번호로 암호화된 항목으로 아카이브를 구성합니다.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
        archive.CreateEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass2", EncryptionMethod.AES128)));
        archive.CreateEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEcryptionSettings("pass3", EncryptionMethod.AES256)));
        archive.Save(zipFile);
    }
}
```

### 또한보십시오

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, ArchiveEntrySettings, FileSystemInfo) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public ArchiveEntry CreateEntry(string name, Stream source, ArchiveEntrySettings newEntrySettings, 
    FileSystemInfo fileInfo)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| source | Stream | 항목의 입력 스트림입니다. |
| newEntrySettings | ArchiveEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`ArchiveEntry`](../../archiveentry/) 안건. |
| fileInfo | FileSystemInfo | 압축할 파일 또는 폴더의 메타데이터입니다. |

### 반환 값

Zip 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| InvalidOperationException | 둘 다*source* 그리고*fileInfo* null이거나*source*null이고*fileInfo* 디렉토리를 나타냅니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*fileInfo* 매개변수는 항목 이름에 영향을 주지 않습니다.

*fileInfo* 참조할 수 있습니다DirectoryInfo 항목이 디렉토리인 경우.

### 예

암호화된 항목으로 아카이브를 작성합니다.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF} ), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new FileInfo("data1.bin")); 
        archive.Save(zipFile);
    }
}
```

### 또한보십시오

* class [ArchiveEntry](../../archiveentry/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* 네임스페이스 [Aspose.Zip](../../archive/)
* 집회 [Aspose.Zip](../../../)


