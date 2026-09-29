---
title: "LzmaArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 LZMA 아카이브 파일을 나타냅니다."
type: docs
weight: 86
url: /ko/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

이 클래스는 LZMA 아카이브 파일을 나타냅니다. 이를 사용하여 LZMA 아카이브를 만들거나 추출할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | 새 인스턴스를 초기화하고 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스를 사용하여 lzma 형식으로 아카이브를 구성합니다. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | 새 인스턴스를 초기화하고 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스를 사용하여 lzma 형식으로 아카이브를 구성합니다. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | 압축 해제를 위해 준비된 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스의 새 인스턴스를 초기화합니다. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | 압축 해제를 위해 준비된 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | lzma 아카이브를 파일로 추출합니다. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | lzma 아카이브를 스트림으로 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 경로를 지정하여 lzma 아카이브를 파일로 추출합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져와 lzma 아카이브를 구성합니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getLength()](#getLength--) | 길이를 가져옵니다. |
| [getName()](#getName--) | 원본 파일의 이름. |
| [save(File destination)](#save-java.io.File-) | 제공된 대상 파일에 lzma 아카이브를 저장합니다. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 제공된 스트림에 lzma 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 lzma 아카이브를 저장합니다. |
| [setSource(File file)](#setSource-java.io.File-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | 아카이브 내에서 압축될 내용을 설정합니다. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


새 인스턴스를 초기화하고 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스를 사용하여 lzma 형식으로 아카이브를 구성합니다.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


새 인스턴스를 초기화하고 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스를 사용하여 lzma 형식으로 아카이브를 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | 특정 lzma 아카이브 설정 집합 |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


압축 해제를 위해 준비된 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스의 새 인스턴스를 초기화합니다.

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


압축 해제를 위해 준비된 [LzmaArchive](../../com.aspose.zip/lzmaarchive) 클래스의 새 인스턴스를 초기화합니다.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일 | java.io.File | 압축 해제된 데이터를 저장할 파일 |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


lzma 아카이브를 스트림으로 추출합니다.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 압축 해제된 데이터를 저장할 파일의 경로 |

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
|  | destinationDirectory | java.lang.String | 압축 해제된 파일을 배치할 디렉터리 경로. |

디렉터리가 존재하지 않으면 생성됩니다 |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


[IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져와 lzma 아카이브를 구성합니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - lzma 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목들.
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
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


제공된 대상 파일에 lzma 아카이브를 저장합니다.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(new File(\"archive.lzma\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 출력 | java.io.OutputStream | 대상 스트림 |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


제공된 대상 파일에 lzma 아카이브를 저장합니다.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save(\"result.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일 | java.io.File | 입력 스트림으로 열릴 파일 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save(\"archive.lzma\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourcePath | java.lang.String | 입력 스트림으로 열릴 파일 경로 |

