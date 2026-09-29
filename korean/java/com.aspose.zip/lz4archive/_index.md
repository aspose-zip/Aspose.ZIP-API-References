---
title: "Lz4Archive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 LZ4 아카이브 파일을 나타냅니다."
type: docs
weight: 80
url: /ko/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

이 클래스는 LZ4 아카이브 파일을 나타냅니다. 이를 사용하여 LZ4 아카이브를 추출하거나 구성할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | 압축 해제를 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다. |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | 압축 해제를 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다. |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다. |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다. |
| [Lz4Archive()](#Lz4Archive--) | 압축을 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다. |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | 압축을 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 아카이브를 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 아카이브를 경로에 따라 파일로 추출합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getLength()](#getLength--) | 길이를 가져옵니다. |
| [getName()](#getName--) | 원본 이름을 가져옵니다. |
| [open()](#open--) | 추출을 위해 아카이브를 열고 아카이브 내용을 포함한 스트림을 제공합니다. |
| [save(File destination)](#save-java.io.File-) | 제공된 대상 파일에 lz4 아카이브를 저장합니다. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 제공된 스트림에 lz4 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(File fileInfo)](#setSource-java.io.File-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(String path)](#setSource-java.lang.String-) | 아카이브 내에서 압축될 내용을 설정합니다. |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


압축 해제를 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다.

스트림에서 아카이브를 열고 이를 `MemoryStream`에 추출합니다.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [open()](../../com.aspose.zip/lz4archive\#open--) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | 아카이브를 로드할 옵션입니다. |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


[Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다.

파일 경로에서 아카이브를 열고 `MemoryStream`으로 추출합니다.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [open()](../../com.aspose.zip/lz4archive\#open--) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | 아카이브를 로드할 옵션입니다. |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


압축을 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다.

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


압축을 위해 준비된 [Lz4Archive](../../com.aspose.zip/lz4archive) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | 구성된 아카이브의 설정입니다. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


제공된 스트림으로 아카이브를 추출합니다.

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

스트림에서 읽어 파일의 원본 내용을 가져옵니다. 예제 섹션을 참조하십시오.

**Returns:**
java.io.InputStream - 아카이브 내용을 나타내는 스트림
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


제공된 대상 파일에 lz4 아카이브를 저장합니다.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File("archive.lz4"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 출력 | java.io.OutputStream | 대상 스트림. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


제공된 대상 파일에 아카이브를 저장합니다.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(\"data.bin\");
archive.save("archive.lz4");
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
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

이 메서드를 사용하여 결합된 tar.lz4 아카이브를 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | 압축할 Tar 아카이브입니다. |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fileInfo | java.io.File | 압축될 파일에 대한 참조입니다. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.lz4");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 압축될 파일의 경로. |

