---
title: "IsoArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "ISO 9660 아카이브를 나타냅니다."
type: docs
weight: 71
url: /ko/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

ISO 아카이브(ISO 9660)를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | 새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 새 파일 및 디렉터리를 추가하기 위한 빈 ISO 아카이브를 생성합니다. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | 새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | 새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | 새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | 새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | ISO 이미지에 디렉터리를 추가합니다. |
| [createEntry(String name)](#createEntry-java.lang.String-) | ISO 이미지에 파일을 추가합니다. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | ISO 이미지에 파일을 추가합니다. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | ISO 이미지에 파일을 추가합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 지정된 디렉터리로 모든 항목을 추출합니다. |
| [getEntries()](#getEntries--) | 아카이브를 구성하는 [IsoEntry](../../com.aspose.zip/isoentry) 유형의 항목을 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | ISO 이미지를 지정된 스트림에 저장합니다. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | ISO 이미지를 지정된 스트림에 저장합니다. |
| [save(String path)](#save-java.lang.String-) | ISO 이미지를 지정된 경로에 저장합니다. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | ISO 이미지를 지정된 경로에 저장합니다. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 새 파일 및 디렉터리를 추가하기 위한 빈 ISO 아카이브를 생성합니다.

다음 예제는 새 빈 ISO 아카이브를 생성하고 파일을 추가하는 방법을 보여줍니다:

```

``````

// 새 빈 ISO 아카이브 생성
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO 아카이브에 파일 추가
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO 아카이브를 파일에 저장
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

이 생성자는 어떤 항목도 풀어내지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

이 생성자는 어떤 항목도 풀어내지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


새로운 [IsoArchive](../../com.aspose.zip/isoarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```

``````

try (IsoArchive archive = new IsoArchive("archive.iso")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 엔트리를 추출할 디렉터리 |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


아카이브를 구성하는 [IsoEntry](../../com.aspose.zip/isoentry) 유형의 항목을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - iso 아카이브를 구성하는 [IsoEntry](../../com.aspose.zip/isoentry) 유형의 항목
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - iso 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


ISO 이미지를 지정된 스트림에 저장합니다.

다음 예제는 ISO 아카이브를 메모리 스트림에 저장하는 방법을 보여줍니다:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// 새 빈 ISO 아카이브 생성
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO 아카이브에 파일 추가
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO 아카이브를 메모리 스트림에 저장
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | ISO 이미지가 저장될 스트림 |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | ISO 아카이브를 저장하기 위한 옵션 |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


ISO 이미지를 지정된 경로에 저장합니다.

다음 예제는 ISO 아카이브를 파일에 저장하는 방법을 보여줍니다:

```

``````

// 새 빈 ISO 아카이브 생성
try (IsoArchive isoArchive = new IsoArchive()) {
// ISO 아카이브에 파일 추가
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// ISO 아카이브를 파일에 저장
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | ISO 이미지가 저장될 경로 |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | ISO 아카이브를 저장하기 위한 옵션 |

