---
title: "UueArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 uuencoded 파일을 나타냅니다."
type: docs
weight: 128
url: /ko/java/com.aspose.zip/uuearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class UueArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

이 클래스는 uuencoded 파일을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [UueArchive()](#UueArchive--) | 인코딩을 위해 준비된 [UueArchive](../../com.aspose.zip/uuearchive) 클래스의 새 인스턴스를 초기화합니다. |
| [UueArchive(InputStream sourceStream)](#UueArchive-java.io.InputStream-) | 디코딩을 위해 준비된 [UueArchive](../../com.aspose.zip/uuearchive) 클래스의 새 인스턴스를 초기화합니다. |
| [UueArchive(String path)](#UueArchive-java.lang.String-) | [UueArchive](../../com.aspose.zip/uuearchive) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | 제공된 스트림으로 아카이브를 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 아카이브를 경로에 따라 파일로 추출합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | uue 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getLength()](#getLength--) | 길이를 가져옵니다. |
| [getName()](#getName--) | 원본 파일의 이름. |
| [open()](#open--) | 아카이브를 디코딩하기 위해 열고 아카이브 콘텐츠가 포함된 스트림을 제공합니다. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(OutputStream outputStream, UueSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [save(String destinationFileName, UueSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.UueSaveOptions-) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [setSource(File file)](#setSource-java.io.File-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 아카이브 내에 인코딩될 콘텐츠를 설정합니다. |
| [setSource(String path)](#setSource-java.lang.String-) | 아카이브 내에 인코딩될 콘텐츠를 설정합니다. |
### UueArchive() {#UueArchive--}
```
public UueArchive()
```


인코딩을 위해 준비된 [UueArchive](../../com.aspose.zip/uuearchive) 클래스의 새 인스턴스를 초기화합니다.

다음 예제는 파일을 uuencode하는 방법을 보여줍니다.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.uue");
}
 
```



### UueArchive(InputStream sourceStream) {#UueArchive-java.io.InputStream-}
```
public UueArchive(InputStream sourceStream)
```


Initializes a new instance of the [UueArchive](../../com.aspose.zip/uuearchive) class prepared for decoding.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (UueArchive archive = new UueArchive(new FileInputStream("archive.001"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

이 생성자는 디코딩하지 않습니다. 압축 해제를 위해 [open()](../../com.aspose.zip/uuearchive\#open--) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |

### UueArchive(String path) {#UueArchive-java.lang.String-}
```
public UueArchive(String path)
```


[UueArchive](../../com.aspose.zip/uuearchive) 클래스의 새 인스턴스를 초기화합니다.

파일 경로에서 아카이브를 열고 `MemoryStream`으로 디코딩합니다.

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (UueArchive archive = new UueArchive(new FileInputStream("archive.uue"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decode. See [open()](../../com.aspose.zip/uuearchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

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

     try (UueArchive archive = new UueArchive("archive.uue")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 대상 스트림 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


아카이브를 경로에 따라 파일로 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 대상 파일의 경로입니다. 파일이 이미 존재하면 덮어쓰게 됩니다. |

**Returns:**
java.io.File - 추출된 파일 정보
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


제공된 디렉터리로 아카이브의 내용을 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | 압축 해제된 파일을 배치할 디렉터리 경로. |

디렉터리가 존재하지 않으면 생성됩니다 |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


uue 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - uue 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목
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


길이를 가져옵니다.

**Returns:**
java.lang.Long - 길이
### getName() {#getName--}
```
public final String getName()
```


원본 파일의 이름.

**Returns:**
java.lang.String - 원본 파일의 이름
### open() {#open--}
```
public final InputStream open()
```


아카이브를 디코딩하기 위해 열고 아카이브 콘텐츠가 포함된 스트림을 제공합니다.

사용법:

```

``````

try (InputStream decompressed = archive.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| outputStream | java.io.OutputStream | 대상 스트림 |

### save(OutputStream outputStream, UueSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.UueSaveOptions-}
```
public final void save(OutputStream outputStream, UueSaveOptions saveOptions)
```


제공된 스트림에 아카이브를 저장합니다.

압축된 데이터를 HTTP 응답 스트림에 씁니다.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves the archive to the destination file provided.

Write encoded data to file.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.uue");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |

### save(String destinationFileName, UueSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.UueSaveOptions-}
```
public final void save(String destinationFileName, UueSaveOptions saveOptions)
```


제공된 대상 파일에 아카이브를 저장합니다.

인코딩된 데이터를 파일에 씁니다.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| saveOptions | [UueSaveOptions](../../com.aspose.zip/uuesaveoptions) | options for the archive saving |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일 | java.io.File | 압축될 파일에 대한 참조 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


아카이브 내에 인코딩될 콘텐츠를 설정합니다.

```

``````

try (UueArchive archive = new UueArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.uue");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be encoded within the archive.

```

``````

     try (UueArchive archive = new UueArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.uue");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 인코딩될 파일의 경로 |

