---
title: "LzxArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 LZX .lzx 아카이브 파일을 나타냅니다."
type: docs
weight: 89
url: /ko/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

이 클래스는 LZX(.lzx) 아카이브 파일을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | 새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | 새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | 새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | 새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 아카이브의 모든 파일 및 디렉터리를 제공된 디렉터리로 추출합니다. |
| [getEntries()](#getEntries--) | 아카이브를 구성하는 [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) 유형의 파일 항목을 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

이 생성자는 어떤 항목도 압축을 해제하지 않습니다. 압축 해제를 위해 [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 아카이브의 소스입니다. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

이 생성자는 어떤 항목도 압축을 해제하지 않습니다. 압축 해제를 위해 [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 아카이브의 소스입니다. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


새로운 [LzxArchive](../../com.aspose.zip/lzxarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

다음 예제는 아카이브를 추출한 다음 첫 번째 항목을 `MemoryStream`으로 압축 해제합니다.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

이 생성자는 어떤 항목도 압축을 해제하지 않습니다. 압축 해제를 위해 [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일에 대한 전체 경로나 상대 경로입니다. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

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

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
