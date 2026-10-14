---
title: "SharArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 shar 아카이브 파일을 나타냅니다."
type: docs
weight: 119
url: /ko/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

이 클래스는 shar 아카이브 파일을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SharArchive()](#SharArchive--) | 새로운 [SharArchive](../../com.aspose.zip/shararchive) 클래스 인스턴스를 초기화합니다. |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | 압축 해제를 위해 준비된 새로운 [SharArchive](../../com.aspose.zip/shararchive) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | 주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | 아카이브 내에 단일 엔트리를 생성합니다. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 아카이브 내에 단일 엔트리를 생성합니다. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | 아카이브 내에 단일 엔트리를 생성합니다. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 아카이브 내에 단일 엔트리를 생성합니다. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | 엔트리 목록에서 특정 엔트리의 첫 번째 발생을 제거합니다. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | 인덱스로 항목 목록에서 해당 항목을 제거합니다. |
| [getEntries()](#getEntries--) | [SharEntry](../../com.aspose.zip/sharentry) 유형의 항목을 가져와 아카이브를 구성합니다. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 아카이브를 저장합니다. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


새로운 [SharArchive](../../com.aspose.zip/shararchive) 클래스 인스턴스를 초기화합니다.

다음 예제는 파일을 압축하는 방법을 보여줍니다.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 디렉터리 | java.io.File | 압축할 디렉터리 |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceDirectory | java.lang.String | 압축할 디렉터리 |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


주어진 디렉터리의 모든 파일과 디렉터리를 재귀적으로 아카이브에 추가합니다.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 항목의 이름 |
| 파일 | java.io.File | 압축될 파일 또는 폴더의 메타데이터 |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


아카이브 내에 단일 엔트리를 생성합니다.

```

``````

java.io.File file = new java.io.File(\"data.bin\");
try (SharArchive archive = new SharArchive()) {
archive.createEntry("test.bin", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 항목의 이름 |
| source | java.io.InputStream | 엔트리의 입력 스트림 |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


아카이브 내에 단일 엔트리를 생성합니다.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

`name` 매개변수 내에서만 엔트리 이름이 설정됩니다. `sourcePath` 매개변수에 제공된 파일 이름은 엔트리 이름에 영향을 주지 않습니다.

`openImmediately` 매개변수로 파일을 즉시 열면 아카이브가 해제될 때까지 파일이 차단됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 항목의 이름 |
| sourcePath | java.lang.String | 압축할 파일의 경로 |
| openImmediately | boolean | true, 파일을 즉시 열 경우, 그렇지 않으면 아카이브 저장 시 파일을 엽니다 |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


엔트리 목록에서 특정 엔트리의 첫 번째 발생을 제거합니다.

다음은 마지막 엔트리를 제외한 모든 엔트리를 제거하는 방법입니다:

```

``````

try (SharArchive archive = new SharArchive("archive.shar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputSharFile.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| entryIndex | int | 제거할 엔트리의 0 기반 인덱스 |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


[SharEntry](../../com.aspose.zip/sharentry) 유형의 항목을 가져와 아카이브를 구성합니다.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - 아카이브를 구성하는 [SharEntry](../../com.aspose.zip/sharentry) 유형의 항목
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


제공된 스트림에 아카이브를 저장합니다.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry("entry1", "data.bin");
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | 생성될 아카이브의 경로입니다. 지정된 파일 이름이 기존 파일을 가리키면 해당 파일이 덮어쓰기됩니다. |

아카이브를 로드된 동일한 경로에 저장할 수 있습니다. 그러나 이 방법은 임시 파일에 복사하는 방식을 사용하므로 권장되지 않습니다 |

