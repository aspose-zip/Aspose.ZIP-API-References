---
title: "LzipArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 Lzip 아카이브 파일을 나타냅니다."
type: docs
weight: 83
url: /ko/java/com.aspose.zip/lziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

이 클래스는 Lzip 아카이브 파일을 나타냅니다. Lzip 아카이브를 만들거나 추출하는 데 사용합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzipArchive()](#LzipArchive--) | 새로운 [LzipArchive](../../com.aspose.zip/lziparchive) 인스턴스를 초기화합니다. |
| [LzipArchive(LzipArchiveSettings settings)](#LzipArchive-com.aspose.zip.LzipArchiveSettings-) | 새로운 [LzipArchive](../../com.aspose.zip/lziparchive) 인스턴스를 초기화합니다. |
| [LzipArchive(InputStream sourceStream)](#LzipArchive-java.io.InputStream-) | 압축 해제를 위해 준비된 [LzipArchive](../../com.aspose.zip/lziparchive) 클래스의 새로운 인스턴스를 초기화합니다. |
| [LzipArchive(InputStream sourceStream, LzipLoadOptions options)](#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-) | 압축 해제를 위해 준비된 [LzipArchive](../../com.aspose.zip/lziparchive) 클래스의 새로운 인스턴스를 초기화합니다. |
| [LzipArchive(String path)](#LzipArchive-java.lang.String-) | 압축 해제를 위해 준비된 [LzipArchive](../../com.aspose.zip/lziparchive) 클래스의 새로운 인스턴스를 초기화합니다. |
| [LzipArchive(String path, LzipLoadOptions options)](#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-) | 압축 해제를 위해 준비된 [LzipArchive](../../com.aspose.zip/lziparchive) 클래스의 새로운 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzip 아카이브를 파일로 추출합니다. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzip 아카이브를 스트림으로 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 경로를 지정하여 lzip 아카이브를 파일로 추출합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | lzip 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getLength()](#getLength--) | 길이를 가져옵니다. |
| [getName()](#getName--) | 원본 파일의 이름. |
| [getSettings()](#getSettings--) | 특정 lzip 아카이브의 설정을 가져옵니다. |
| [getUncompressedSize()](#getUncompressedSize--) | 파일 데이터의 압축 해제된 크기를 바이트 단위로 가져옵니다. |
| [save(File destination)](#save-java.io.File-) | 제공된 대상 파일에 lzip 아카이브를 저장합니다. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | 제공된 스트림에 lzip 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 lzip 아카이브를 저장합니다. |
| [setSource(File file)](#setSource-java.io.File-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(String path)](#setSource-java.lang.String-) | 아카이브 내에서 압축될 내용을 설정합니다. |
### LzipArchive() {#LzipArchive--}
```
public LzipArchive()
```


새로운 [LzipArchive](../../com.aspose.zip/lziparchive) 인스턴스를 초기화합니다.

### LzipArchive(LzipArchiveSettings settings) {#LzipArchive-com.aspose.zip.LzipArchiveSettings-}
```
public LzipArchive(LzipArchiveSettings settings)
```


새로운 [LzipArchive](../../com.aspose.zip/lziparchive) 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| settings | [LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) | 사전 크기 정의가 포함된 특정 lzip 아카이브의 설정 |

### LzipArchive(InputStream sourceStream) {#LzipArchive-java.io.InputStream-}
```
public LzipArchive(InputStream sourceStream)
```


압축 해제를 위해 준비된 [LzipArchive](../../com.aspose.zip/lziparchive) 클래스의 새로운 인스턴스를 초기화합니다.

```

``````

try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### LzipArchive(InputStream sourceStream, LzipLoadOptions options) {#LzipArchive-java.io.InputStream-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(InputStream sourceStream, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | 아카이브를 로드하기 위한 옵션. |

### LzipArchive(String path) {#LzipArchive-java.lang.String-}
```
public LzipArchive(String path)
```


압축 해제를 위해 준비된 [LzipArchive](../../com.aspose.zip/lziparchive) 클래스의 새로운 인스턴스를 초기화합니다.

```

``````

try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
archive.extract(extractedFile);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### LzipArchive(String path, LzipLoadOptions options) {#LzipArchive-java.lang.String-com.aspose.zip.LzipLoadOptions-}
```
public LzipArchive(String path, LzipLoadOptions options)
```


Initializes a new instance of the [LzipArchive](../../com.aspose.zip/lziparchive) class prepared for decompressing.

```

``````

     try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
         try (LzipArchive archive = new LzipArchive("sourceLzipFileName")) {
             archive.extract(extractedFile);
         }
     } catch (IOException ex) {
     }
 
```

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(OutputStream)](../../com.aspose.zip/lziparchive\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 소스의 경로 |
| options | [LzipLoadOptions](../../com.aspose.zip/lziploadoptions) | 아카이브를 로드하기 위한 옵션. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


lzip 아카이브를 파일로 추출합니다.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzip archive to a stream.

```

``````

     try (FileInputStream sourceLzipFile = new FileInputStream("sourceLzipFile")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (LzipArchive archive = new LzipArchive(sourceLzipFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.OutputStream | 압축 해제된 데이터를 저장하기 위한 스트림 |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


경로를 지정하여 lzip 아카이브를 파일로 추출합니다.

```

``````

try (FileInputStream lzipFile = new FileInputStream("sourceFileName")) {
try (LzipArchive archive = new LzipArchive(lzipFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzip archive
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


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### getSettings() {#getSettings--}
```
public final LzipArchiveSettings getSettings()
```


Gets the setting of particular lzip archive.

**Returns:**
[LzipArchiveSettings](../../com.aspose.zip/lziparchivesettings) - the setting of particular lzip archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the uncompressed size of the file data in bytes.

**Returns:**
long - the uncompressed size of the file data in bytes
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lz"));
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대상 | java.io.File | 대상 스트림으로 열릴 파일 |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


제공된 스트림에 lzip 아카이브를 저장합니다.

```

``````

try (FileOutputStream lzFile = new FileOutputStream("archive.lz")) {
try (LzipArchive archive = new LzipArchive()) {
archive.setSource(\"data.bin\");
archive.save(lzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzip archive to destination file provided.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lz");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzipArchive archive = new LzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {0x00, (byte)0xFF} ));
         archive.save("archive.lz");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브용 입력 스트림 |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (LzipArchive archive = new LzipArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.lz");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file to be compressed |

