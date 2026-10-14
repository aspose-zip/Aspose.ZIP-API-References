---
title: "RarArchiveEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "아카이브 내 단일 파일을 나타냅니다."
type: docs
weight: 98
url: /ko/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

아카이브 내 단일 파일을 나타냅니다.

인스턴스를 [RarArchiveEntry](../../com.aspose.zip/rararchiveentry)에서 [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted)으로 캐스팅하여 해당 항목이 암호화되었는지 여부를 확인합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getCompressedSize()](#getCompressedSize--) | 압축된 파일의 크기를 가져옵니다. |
| [getCreationTime()](#getCreationTime--) | 생성 날짜와 시간을 가져옵니다. |
| [getExtractionProgressed()](#getExtractionProgressed--) | 원시 스트림의 일부가 추출될 때 발생하는 이벤트를 가져옵니다. |
| [getLastAccessTime()](#getLastAccessTime--) | 마지막 액세스 날짜와 시간을 가져옵니다. |
| [getLength()](#getLength--) | 길이를 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 마지막 수정 날짜와 시간을 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 항목의 이름을 가져옵니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 원본 파일의 크기를 가져옵니다. |
| [isDirectory()](#isDirectory--) | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [open()](#open--) | 추출을 위해 항목을 열고 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |
| [open(String password)](#open-java.lang.String-) | 추출을 위해 항목을 열고 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 원시 스트림의 일부가 추출될 때 발생하는 이벤트를 설정합니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


제공된 스트림으로 항목을 추출합니다.


비밀번호로 rar 아카이브의 항목을 추출합니다.

```

``````

try (FileInputStream rarFile = new FileInputStream(\"archive.rar\")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(outputStream, \"p@s$\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림. 쓰기 가능해야 합니다. |
| password | java.lang.String | 복호화를 위한 선택적 비밀번호. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다.


rar 아카이브의 두 항목을 추출합니다.

```

``````

try (FileInputStream rarFile = new FileInputStream(\"archive.rar\")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract(\"first.bin\", \"pass\");
archive.getEntries().get(1).extract(\"second.bin\", \"pass\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로. 파일이 이미 존재하면 덮어쓰게 됩니다. |
| password | java.lang.String | 복호화를 위한 선택적 비밀번호. |

**Returns:**
java.io.File - 추출된 파일의 파일 정보
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


압축된 파일의 크기를 가져옵니다.

**Returns:**
long - 압축된 파일의 크기
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


생성 날짜와 시간을 가져옵니다.

**Returns:**
java.util.Date - 생성 날짜와 시간.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


원시 스트림의 일부가 추출될 때 발생하는 이벤트를 가져옵니다.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

스트림에서 읽어 파일의 원본 내용을 가져옵니다. 예제 섹션을 참조하세요.

**Returns:**
java.io.InputStream - 항목의 내용을 나타내는 스트림입니다.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


추출을 위해 항목을 열고 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다.


사용법:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

Event sender는 [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) 인스턴스입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 원시 스트림의 일부가 추출될 때 발생하는 이벤트입니다. |

