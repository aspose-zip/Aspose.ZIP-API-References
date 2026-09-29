---
title: "GzipArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 gzip 아카이브 파일을 나타냅니다."
type: docs
weight: 69
url: /ko/java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

이 클래스는 gzip 아카이브 파일을 나타냅니다. gzip 아카이브를 생성하거나 추출하는 데 사용합니다.

Gzip 압축 알고리즘은 DEFLATE 알고리즘을 기반으로 하며, 이는 LZ77과 허프만 코딩의 조합입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | 압축을 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | 압축 해제를 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | 압축 해제를 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | 압축 해제를 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | 압축 해제를 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 아카이브를 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 아카이브를 경로에 따라 파일로 추출합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져와 gzip 아카이브를 구성합니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getLength()](#getLength--) | 원본 파일의 크기를 가져옵니다. |
| [getName()](#getName--) | 원본 파일의 이름입니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 원본 파일의 크기를 가져옵니다. |
| [open()](#open--) | 추출을 위해 아카이브를 열고 아카이브 내용을 포함한 스트림을 제공합니다. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(File file)](#setSource-java.io.File-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(String path)](#setSource-java.lang.String-) | 아카이브 내에서 압축될 내용을 설정합니다. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


압축을 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다.

다음 예제는 파일을 압축하는 방법을 보여줍니다.

```

``````

try (GzipArchive archive = new GzipArchive())
{
archive.setSource(\"data.bin\");
archive.save(\"archive.gz\");
}
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [open()](../../com.aspose.zip/gziparchive\\#open--) 메서드를 참조하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스입니다. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


압축 해제를 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다.

스트림에서 아카이브를 열고 `ByteArrayOutputStream`에 추출합니다

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get(\"archive.gz\")))) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [open()](../../com.aspose.zip/gziparchive\\#open--) 메서드를 참조하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스입니다. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | 아카이브를 로드하기 위한 옵션. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


압축 해제를 위해 준비된 새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다.

파일 경로에서 아카이브를 열고 `MemoryStream`으로 추출합니다.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
GzipLoadOptions options = new GzipLoadOptions();
try (GzipArchive archive = new GzipArchive(\"archive.gz\", options)) {
archive.extract(ms);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [open()](../../com.aspose.zip/gziparchive\\#open--) 메서드를 참조하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


새로운 [GzipArchive](../../com.aspose.zip/gziparchive) 클래스 인스턴스를 초기화합니다.

파일 경로에서 아카이브를 열고 `MemoryStream`으로 추출합니다.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (GzipArchive archive = new GzipArchive(\"archive.gz\")) {
byte[] b = new byte[8192];
int bytesRead;
InputStream archiveStream = archive.open();
while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림. 쓰기 가능해야 합니다. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


아카이브를 경로에 따라 파일로 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로. 파일이 이미 존재하면 덮어쓰게 됩니다. |

**Returns:**
java.io.File - 추출된 파일의 파일 정보
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


제공된 디렉터리로 아카이브의 내용을 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 추출된 파일을 배치할 디렉터리 경로입니다. |

디렉터리가 존재하지 않으면 생성됩니다. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져와 gzip 아카이브를 구성합니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - gzip 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목들.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


원본 파일의 크기를 가져옵니다.

압축 해제 중에 이 속성은 잘못된 크기를 포함할 수 있습니다. 압축 해제된 파일 크기가 4GB를 초과하면 헤더의 32비트 제한으로 인해 이 속성이 잘못된 값을 반환합니다.

**Returns:**
java.lang.Long - 원본 파일의 크기
### getName() {#getName--}
```
public final String getName()
```


원본 파일의 이름입니다.

**Returns:**
java.lang.String - 원본 파일의 이름
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


원본 파일의 크기를 가져옵니다.

압축 해제 중에 이 속성은 잘못된 크기를 포함할 수 있습니다. 압축 해제된 파일 크기가 4GB를 초과하면 헤더의 32비트 제한으로 인해 이 속성이 잘못된 값을 반환합니다.

**Returns:**
long - 원본 파일의 크기.
### open() {#open--}
```
public final InputStream open()
```


추출을 위해 아카이브를 열고 아카이브 내용을 포함한 스트림을 제공합니다.

아카이브를 추출하고 추출된 내용을 파일 스트림에 복사합니다.

```

``````

try (GzipArchive archive = new GzipArchive(\"archive.gz\")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputStream | java.io.OutputStream | 대상 스트림. |

`outputStream`은 쓰기 가능해야 합니다. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


제공된 대상 파일에 아카이브를 저장합니다.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save(\"archive.gz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

이 메서드를 사용하여 결합된 tar.gz 아카이브를 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 압축할 Tar 아카이브입니다. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"archive.gz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브용 입력 스트림. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


아카이브 내에서 압축될 내용을 설정합니다.

파일 경로에서 아카이브를 열고 `MemoryStream`으로 추출합니다.

```

``````

try (GzipArchive archive = new GzipArchive()) {
archive.setSource(\"data.bin\");
archive.save(\"archive.gz\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

