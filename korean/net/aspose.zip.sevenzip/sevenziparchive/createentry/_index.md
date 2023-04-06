---
title: SevenZipArchive.CreateEntry
second_title: .NET API 참조용 Aspose.ZIP
description: SevenZipArchive 방법. 아카이브 내에 단일 항목을 생성합니다.
type: docs
weight: 50
url: /ko/net/aspose.zip.sevenzip/sevenziparchive/createentry/
---
## CreateEntry(string, FileInfo, bool, SevenZipEntrySettings) {#createentry}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, FileInfo fileInfo, 
    bool openImmediately = false, SevenZipEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| fileInfo | FileInfo | 압축할 파일의 메타데이터입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |
| newEntrySettings | SevenZipEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) 안건. |

### 반환 값

Seven Zip 항목 인스턴스.

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

각각 다른 비밀번호로 암호화된 항목으로 아카이브를 구성합니다.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    FileInfo fi1 = new FileInfo("data1.bin");
    FileInfo fi2 = new FileInfo("data2.bin");
    FileInfo fi3 = new FileInfo("data3.bin");
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", fi1, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test1")));
        archive.CreateEntry("entry2.bin", fi2, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test2")));
        archive.CreateEntry("entry3.bin", fi3, false, new SevenZipEntrySettings(new SevenZipStoreCompressionSettings(), new SevenZipAESEncryptionSettings("test3")));
        archive.Save(sevenZipFile);
    }
}
```

### 또한보십시오

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings, FileSystemInfo) {#createentry_2}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings, FileSystemInfo fileInfo)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| source | Stream | 항목의 입력 스트림입니다. |
| newEntrySettings | SevenZipEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) 안건. |
| fileInfo | FileSystemInfo | 압축할 파일 또는 폴더의 메타데이터입니다. |

### 반환 값

SevenZip 항목 인스턴스.

### 예외

| 예외 | 상태 |
| --- | --- |
| InvalidOperationException | 둘 다*source* 그리고*fileInfo* null이거나*source*null이고*fileInfo* 디렉토리를 나타냅니다. |

### 비고

항목 이름은 단독으로 설정됩니다.*name* 매개변수. 에 제공된 파일 이름*fileInfo* 매개변수는 항목 이름에 영향을 주지 않습니다.

*fileInfo* 참조할 수 있습니다DirectoryInfo 항목이 디렉토리인 경우.

### 예

LZMA2 압축 암호화 항목으로 아카이브를 작성합니다.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("entry1.bin", new MemoryStream(new byte[] {0x00, 0xFF}), new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("test1")), new FileInfo("data1.bin")); 
        archive.Save(sevenZipFile);
    }
}
```

### 또한보십시오

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, SevenZipEntrySettings) {#createentry_1}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, Stream source, 
    SevenZipEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| source | Stream | 항목의 입력 스트림입니다. |
| newEntrySettings | SevenZipEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) 안건. |

### 반환 값

Zip 항목 인스턴스.

### 예

모든 항목의 LZMA2 압축 및 암호화를 사용하여 7z 아카이브를 작성합니다.

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings(), new SevenZipAESEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", new MemoryStream(new byte[] {0x00, 0xFF} ));
    archive.Save("archive.7z");
}
```

### 또한보십시오

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, SevenZipEntrySettings) {#createentry_3}

아카이브 내에 단일 항목을 생성합니다.

```csharp
public SevenZipArchiveEntry CreateEntry(string name, string path, bool openImmediately = false, 
    SevenZipEntrySettings newEntrySettings = null)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| name | String | 항목의 이름입니다. |
| path | String | 새 파일의 정규화된 이름 또는 압축할 상대 파일 이름입니다. |
| openImmediately | Boolean | 파일을 즉시 열면 True이고, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |
| newEntrySettings | SevenZipEntrySettings | 추가에 사용되는 압축 및 암호화 설정[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) 안건. |

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
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMA2CompressionSettings())))
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### 또한보십시오

* class [SevenZipArchiveEntry](../../sevenziparchiveentry/)
* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* 네임스페이스 [Aspose.Zip.SevenZip](../../sevenziparchive/)
* 집회 [Aspose.Zip](../../../)


