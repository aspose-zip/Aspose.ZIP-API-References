---
title: "ZArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 Z 압축 아카이브 파일을 나타냅니다."
type: docs
weight: 153
url: /ko/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

이 클래스는 Z (compress) 아카이브 파일을 나타냅니다. 이를 사용하여 Z 아카이브를 구성하거나 추출할 수 있습니다.

보십시오 [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ZArchive()](#ZArchive--) | 압축을 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | 압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | 압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | 압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | 압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Z 아카이브를 파일로 추출합니다. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Z 아카이브를 스트림으로 추출합니다. |
| [extract(String path)](#extract-java.lang.String-) | 경로를 지정하여 Z 아카이브를 파일로 추출합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 내용을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져와 Z 아카이브를 구성합니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getLength()](#getLength--) | 항목의 길이를 바이트 단위로 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 엔트리의 이름을 가져옵니다. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 제공된 스트림에 Z 아카이브를 저장합니다. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | 제공된 스트림에 Z 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 Z 아카이브를 저장합니다. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | 제공된 대상 파일에 Z 아카이브를 저장합니다. |
| [setSource(File file)](#setSource-java.io.File-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | 아카이브 내에서 압축될 내용을 설정합니다. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | 아카이브 내에서 압축될 내용을 설정합니다. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


압축을 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다.

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다.

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | 아카이브를 로드하기 위한 옵션 |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다.

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 소스의 경로 |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


압축 해제를 위해 준비된 [ZArchive](../../com.aspose.zip/zarchive) 클래스의 새 인스턴스를 초기화합니다.

이 생성자는 압축을 해제하지 않습니다. 압축 해제를 위해 [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 소스의 경로 |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | 아카이브를 로드하기 위한 옵션 |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Z 아카이브를 파일로 추출합니다.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
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


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
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


경로를 지정하여 Z 아카이브를 파일로 추출합니다.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
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


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 출력 | java.io.OutputStream | 대상 스트림 |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


제공된 스트림에 Z 아카이브를 저장합니다.

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource(\"data.bin\");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


제공된 대상 파일에 Z 아카이브를 저장합니다.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File(\"data.bin\"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일 | java.io.File | 입력 스트림으로 열릴 파일 정보 |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


아카이브 내에서 압축될 내용을 설정합니다.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourcePath | java.lang.String | 입력 스트림으로 열릴 파일의 경로 |

