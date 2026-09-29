---
title: "LhaArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 LHA .lzh 아카이브 파일을 나타냅니다."
type: docs
weight: 75
url: /ko/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

이 클래스는 LHA(.lzh) 아카이브 파일을 나타냅니다.

다음 압축 방법만 지원됩니다:

| ------ | --------------------------------------------- |
| 메서드 | 설명                                   |
| lh0    | 압축되지 않음                                  |
| lh4    | 8 KiB 슬라이딩 사전 및 정적 허프만   |
| lh5    | 16 KiB 슬라이딩 사전 및 정적 허프만  |
| lh6    | 64 KiB 슬라이딩 사전 및 정적 허프만  |
| lh7    | 128 KiB 슬라이딩 사전 및 정적 허프만 |
| lhx    | 1 Mib 슬라이딩 사전 및 정적 허프만   |
| lhd    | 디렉터리                                     |
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | 새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | 새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | 새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | 새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 아카이브의 모든 파일 및 디렉터리를 제공된 디렉터리로 추출합니다. |
| [getEntries()](#getEntries--) | 아카이브를 구성하는 [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) 유형의 파일 항목을 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

이 생성자는 어떤 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

이 생성자는 어떤 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


새 인스턴스를 초기화하고, [LhaArchive](../../com.aspose.zip/lhaarchive) 클래스의 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

다음 예제는 아카이브를 추출한 다음 첫 번째 항목을 `MemoryStream`으로 압축 해제합니다.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

이 생성자는 어떠한 항목도 압축을 해제하지 않습니다. 압축 해제를 위해 [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일에 대한 전체 경로나 상대 경로 |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


아카이브의 모든 파일 및 디렉터리를 제공된 디렉터리로 추출합니다.

```

``````

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
