---
title: "TarArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 tar 아카이브 파일을 나타냅니다."
type: docs
weight: 125
url: /ko/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

이 클래스는 tar 아카이브 파일을 나타냅니다. 이를 사용하여 tar 아카이브를 구성, 추출 또는 업데이트할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TarArchive()](#TarArchive--) | [TarArchive](../../com.aspose.zip/tararchive) 클래스의 새 인스턴스를 초기화합니다. |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | [Archive](../../com.aspose.zip/archive) 클래스의 새 인스턴스를 초기화하고, 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | [TarArchive](../../com.aspose.zip/tararchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 아카이브 내에 단일 항목을 생성합니다. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | 엔트리 목록에서 특정 엔트리의 첫 번째 발생을 제거합니다. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | 인덱스로 항목 목록에서 해당 항목을 제거합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 모든 파일을 추출합니다. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | 제공된 gzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | 제공된 gzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | 제공된 LZ4 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | 제공된 LZ4 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | 제공된 LZMA 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | 제공된 LZMA 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | 제공된 lzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | 제공된 lzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | 제공된 xz 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromXz(String path)](#fromXz-java.lang.String-) | 제공된 xz 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | 제공된 Z 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromZ(String path)](#fromZ-java.lang.String-) | 제공된 Z 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | 제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | 제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다. |
| [getEntries()](#getEntries--) | 아카이브를 구성하는 [TarEntry](../../com.aspose.zip/tarentry) 유형의 엔트리를 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | tar 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 엔트리를 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | 제공된 대상 파일에 아카이브를 저장합니다. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | gzip 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | gzip 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | gzip 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | gzip 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | LZ4 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | LZ4 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | LZ4 압축을 사용하여 경로별 파일에 아카이브를 저장합니다. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | LZ4 압축을 사용하여 경로별 파일에 아카이브를 저장합니다. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | LZMA 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | LZMA 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | lzma 압축을 사용하여 경로별 파일에 아카이브를 저장합니다. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | lzma 압축을 사용하여 경로별 파일에 아카이브를 저장합니다. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | lzip 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | lzip 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | lzip 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | lzip 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | xz 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | xz 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | xz 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | xz 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | xz 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | xz 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Z 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Z 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Z 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Z 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Zstandard 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Zstandard 압축을 사용하여 스트림에 아카이브를 저장합니다. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Zstandard 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Zstandard 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


[TarArchive](../../com.aspose.zip/tararchive) 클래스의 새 인스턴스를 초기화합니다.

다음 예제는 파일을 압축하는 방법을 보여줍니다.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save("archive.tar");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

이 생성자는 어떤 항목도 풀어내지 않습니다. 풀어내기 위해서는 [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


[TarArchive](../../com.aspose.zip/tararchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 엔트리 목록을 구성합니다.

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```

``````

try (TarArchive archive = new TarArchive("archive.tar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 디렉터리 | java.io.File | 압축할 디렉터리 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 압축할 디렉터리 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

엔트리 이름은 `name` 매개변수 내에서만 설정됩니다. `file` 매개변수에 제공된 파일 이름은 엔트리 이름에 영향을 주지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 항목의 이름 |
| 파일 | java.io.File | 압축될 파일 또는 폴더의 메타데이터 |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


아카이브 내에 단일 항목을 생성합니다.

```

``````

File fi = new File("data.bin");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

항목 이름은 `name` 매개변수 안에서만 설정됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 항목의 이름 |
| source | java.io.InputStream | 엔트리의 입력 스트림 |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


아카이브 내에 단일 항목을 생성합니다.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

`name` 매개변수 내에서만 항목 이름이 설정됩니다. `path` 매개변수에 제공된 파일 이름은 항목 이름에 영향을 주지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 항목의 이름 |
| path | java.lang.String | 압축할 파일 경로 |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


아카이브 내에 단일 항목을 생성합니다.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | 항목 목록에서 제거할 항목 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


인덱스로 항목 목록에서 해당 항목을 제거합니다.

```

``````

try (TarArchive archive = new TarArchive("two_files.tar")) {
archive.deleteEntry(0);
archive.save("single_file.tar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

디렉터리가 존재하지 않으면 생성됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 추출된 파일을 배치할 디렉터리 경로 |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


제공된 gzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: gzip 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하십시오.

GZip 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출할 수 있는 기능을 제공하므로, 내부적으로 탐색 가능한 스트림을 사용해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


제공된 gzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: gzip 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하십시오.

GZip 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출할 수 있는 기능을 제공하므로, 내부적으로 탐색 가능한 스트림을 사용해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


제공된 LZ4 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: LZ4 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | source | java.io.InputStream | 아카이브의 소스입니다. |

LZ4 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


제공된 LZ4 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: LZ4 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 아카이브 파일의 경로. |

LZ4 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


제공된 LZMA 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: LZMA 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

LZMA 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


제공된 LZMA 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: LZMA 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

LZMA 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


제공된 lzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: lzip 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

Lzip 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


제공된 lzip 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: lzip 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

Lzip 추출 스트림은 압축 알고리즘의 특성상 탐색이 불가능합니다. Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


제공된 xz 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: xz 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


제공된 xz 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: xz 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

Tar 아카이브는 임의 레코드를 추출하는 기능을 제공하므로 내부적으로 탐색 가능한 스트림을 사용해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


제공된 Z 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: Z 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


제공된 Z 형식 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: Z 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: Zstandard 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| source | java.io.InputStream | 아카이브의 소스 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


제공된 Zstandard 아카이브를 추출하고 추출된 데이터로부터 [TarArchive](../../com.aspose.zip/tararchive)를 구성합니다.

중요: Zstandard 아카이브는 이 메서드 내에서 완전히 추출되며, 내용은 내부에 보관됩니다. 메모리 사용량에 유의하세요.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


아카이브를 구성하는 [TarEntry](../../com.aspose.zip/tarentry) 유형의 엔트리를 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - 아카이브를 구성하는 [TarEntry](../../com.aspose.zip/tarentry) 유형의 항목들
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


tar 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 엔트리를 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - tar 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목들
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


제공된 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`은(는) 쓰기 가능해야 합니다 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


제공된 대상 파일에 아카이브를 저장합니다.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

아카이브를 로드된 동일한 경로에 저장할 수 있습니다. 그러나 이 방법은 임시 파일에 복사하는 방식을 사용하므로 권장되지 않습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


gzip 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`은(는) 쓰기 가능해야 합니다 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


gzip 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


LZ4 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 출력 | java.io.OutputStream | 대상 스트림. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


LZ4 압축을 사용하여 경로별 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키는 경우, 해당 파일이 덮어쓰기됩니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


LZMA 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

중요: tar 아카이브가 이 메서드 내에서 구성된 후 압축됩니다. 내용은 내부에 보관됩니다. 메모리 사용량에 주의하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`은(는) 쓰기 가능해야 합니다 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


lzma 압축을 사용하여 경로별 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

중요: tar 아카이브가 이 메서드 내에서 구성된 후 압축됩니다. 내용은 내부에 보관됩니다. 메모리 사용량에 주의하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


lzip 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`은(는) 쓰기 가능해야 합니다 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


lzip 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


xz 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`스트림은 쓰기 가능해야 합니다 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


xz 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


xz 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | 특정 xz 아카이브 설정 집합: 사전 크기, 블록 크기, 체크 유형 |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Z 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 출력 | java.io.OutputStream | 대상 스트림 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Z 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Zstandard 압축을 사용하여 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`은(는) 쓰기 가능해야 합니다 |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Zstandard 압축을 사용하여 경로로 지정된 파일에 아카이브를 저장합니다.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 생성될 아카이브의 경로. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰여집니다. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | tar 헤더 형식을 정의합니다. 가능한 경우 null 값은 USTar로 처리됩니다. |

