---
title: "ArchiveEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "아카이브 내 단일 파일을 나타냅니다."
type: docs
weight: 27
url: /ko/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

아카이브 내 단일 파일을 나타냅니다.

항목이 암호화되었는지 여부를 확인하기 위해 [ArchiveEntry](../../com.aspose.zip/archiveentry) 인스턴스를 [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) 로 캐스팅합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | 제공된 스트림으로 항목을 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | 제공된 경로를 사용하여 파일 시스템에 항목을 추출합니다. |
| [getComment()](#getComment--) | 아카이브 내 항목의 주석을 가져옵니다. |
| [getCompressedSize()](#getCompressedSize--) | 압축된 파일의 크기를 가져옵니다. |
| [getCompressionProgressed()](#getCompressionProgressed--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다. |
| [getCompressionSettings()](#getCompressionSettings--) | 압축 또는 압축 해제를 위한 설정을 가져옵니다. |
| [getDataSource()](#getDataSource--) | 항목이 아카이브에 추가된 경우의 소스이며, 추출된 것이 아닙니다. |
| [getExtractionProgressed()](#getExtractionProgressed--) | 원시 스트림의 일부가 추출될 때 발생하는 이벤트를 가져옵니다. |
| [getLength()](#getLength--) | 길이를 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 마지막 수정 날짜와 시간을 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 항목의 이름을 가져옵니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 원본 파일의 크기를 가져옵니다. |
| [isDirectory()](#isDirectory--) | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [open()](#open--) | 추출을 위해 항목을 열고 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |
| [open(String password)](#open-java.lang.String-) | 추출을 위해 항목을 열고 압축 해제된 항목 내용을 포함하는 스트림을 제공합니다. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | 원시 스트림의 일부가 압축될 때 발생하는 이벤트를 설정합니다. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | 원시 스트림의 일부가 추출될 때 발생하는 이벤트를 설정합니다. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | 마지막 수정 날짜와 시간을 설정합니다. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


제공된 스트림으로 항목을 추출합니다.

비밀번호를 사용하여 zip 아카이브의 항목을 추출합니다.

```

``````

try (FileInputStream zipFile = new FileInputStream(\"archive.zip\")) {
try (Archive archive = new Archive(zipFile)) {
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

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
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

각각 고유한 비밀번호를 사용하여 ZIP 아카이브의 두 항목을 추출합니다.

```

``````

try (FileInputStream zipFile = new FileInputStream(\"archive.zip\")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(\"first.bin\", \"first_pass\");
archive.getEntries().get(1).extract(\"second.bin\", \"second_pass\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
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
### getComment() {#getComment--}
```
public final String getComment()
```


아카이브 내 항목의 주석을 가져옵니다.

**Returns:**
java.lang.String - 아카이브 내 항목의 주석
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


압축된 파일의 크기를 가져옵니다.

**Returns:**
long - 압축된 파일의 크기
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


원시 스트림의 일부가 압축될 때 발생하는 이벤트를 가져옵니다.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

이 샘플에서는 항목이 처음 100MB가 추출된 후 취소를 위해 이벤트 핸들러를 사용합니다.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
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

스트림을 읽어 파일의 원본 내용을 가져옵니다.

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
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

Event sender는 [ArchiveEntry](../../com.aspose.zip/archiveentry) 인스턴스입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | 원시 스트림의 일부가 압축될 때 발생하는 이벤트입니다. |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


원시 스트림의 일부가 추출될 때 발생하는 이벤트를 설정합니다.

이 샘플에서는 진행된 크기의 비율을 백분율로 계산하기 위해 이벤트 핸들러를 사용합니다.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender는 [ArchiveEntry](../../com.aspose.zip/archiveentry) 인스턴스입니다. 추출을 취소할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | 원시 스트림의 일부가 추출될 때 발생하는 이벤트입니다. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


마지막 수정 날짜와 시간을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 마지막 수정 날짜 및 시간 |

