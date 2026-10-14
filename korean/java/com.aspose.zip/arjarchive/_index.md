---
title: "ArjArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 ARJ 아카이브 파일을 나타냅니다."
type: docs
weight: 37
url: /ko/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

이 클래스는 ARJ 아카이브 파일을 나타냅니다.

다음 압축 방법만 지원됩니다:

| ------ | ------------------------------------------------------------ |
| 방법 | 설명                                                  |
| 0      | 압축되지 않음                                                 |
| 1      | LZ77와 적응형 허프만 코딩의 조합. 최상의 비율. |
| 2      | LZ77와 적응형 허프만 코딩의 조합.             |
| 3      | LZ77와 적응형 허프만 코딩의 조합. 최상의 속도. |
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | 새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | 새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | 새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | 새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 지정된 디렉터리로 모든 항목을 추출합니다. |
| [getCommentary()](#getCommentary--) | 주석을 가져옵니다. |
| [getEntries()](#getEntries--) | ARJ 아카이브를 구성하는 [ArjEntryPlain](../../com.aspose.zip/arjentryplain) 유형의 엔트리를 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getName()](#getName--) | 원본 이름을 가져옵니다. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다.

이 생성자는 어떤 엔트리도 압축 해제하지 않습니다. 압축 해제를 위해 [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 아카이브의 소스 |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다.

이 생성자는 어떤 엔트리도 압축 해제하지 않습니다. 압축 해제를 위해 [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| extractionSource | java.io.InputStream | 아카이브의 소스 |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


새로운 [ArjArchive](../../com.aspose.zip/arjarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다.

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

이 생성자는 어떤 엔트리도 풀어내지 않습니다. 압축 해제를 위해 [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


지정된 디렉터리로 모든 항목을 추출합니다.

다음 예제는 모든 엔트리를 디렉터리로 추출하는 방법을 보여줍니다:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
