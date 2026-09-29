---
title: "AppleArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 Apple Archive .aar 파일을 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

이 클래스는 Apple Archive (.aar) 파일을 나타냅니다. Apple Archive 파일을 만들 때 사용하십시오.

Apple 및 Apple Archive는 Apple Inc.의 상표입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | 조합된 항목에 사용되는 설정으로 [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화합니다. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | 조합된 항목에 사용되는 설정으로 [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화합니다. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | 지정된 디렉터리의 모든 파일 및 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | 지정된 디렉터리의 모든 파일 및 디렉터리를 재귀적으로 아카이브에 추가합니다. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | 아카이브 내에 단일 항목을 생성합니다. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | 아카이브 내에 단일 항목을 생성합니다. |
| [dispose()](#dispose--) | 관리되지 않는 리소스를 해제하거나, 릴리스하거나, 재설정하는 애플리케이션 정의 작업을 수행합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 모든 파일을 추출합니다. |
| [getEntries()](#getEntries--) | 아카이브를 구성하는 항목을 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getNewEntrySettings()](#getNewEntrySettings--) | 새로 구성된 항목에 사용되는 설정을 가져옵니다. |
| [isSolid()](#isSolid--) | 아카이브가 솔리드 압축을 사용하는지 여부를 나타내는 값을 가져옵니다. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | 제공된 스트림에 아카이브를 저장합니다. |
| [save(String destinationFileName)](#save-java.lang.String-) | 제공된 대상 파일에 아카이브를 저장합니다. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


조합된 항목에 사용되는 설정으로 [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화합니다.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


조합된 항목에 사용되는 설정으로 [AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | 새 Apple Archive를 구성할 때 사용되는 설정입니다. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


[AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | 아카이브의 소스입니다. |

이 생성자는 어떠한 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 및 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 메서드를 참조하십시오. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


[AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스입니다. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

이 생성자는 어떠한 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 및 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 메서드를 참조하십시오. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


[AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 아카이브 파일에 대한 전체 경로나 상대 경로입니다. |

이 생성자는 어떠한 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 및 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 메서드를 참조하십시오. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


[AppleArchive](../../com.aspose.zip/applearchive) 클래스의 새 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일에 대한 전체 경로나 상대 경로입니다. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

이 생성자는 어떠한 항목도 압축 해제하지 않습니다. 압축 해제를 위해 [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) 및 [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) 메서드를 참조하십시오. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


지정된 디렉터리의 모든 파일 및 디렉터리를 재귀적으로 아카이브에 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 디렉터리 | java.io.File | 압축할 디렉터리. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


지정된 디렉터리의 모든 파일 및 디렉터리를 재귀적으로 아카이브에 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 디렉터리 | java.io.File | 압축할 디렉터리. |
| includeRootDirectory | boolean | 루트 디렉터리를 포함할지 여부를 나타냅니다. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


아카이브 내에 단일 항목을 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 엔트리의 이름. |
| fileInfo | java.io.File | 압축될 파일의 메타데이터. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


아카이브 내에 단일 항목을 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 엔트리의 이름. |
| fileInfo | java.io.File | 압축될 파일의 메타데이터. |
| openImmediately | boolean | 파일을 즉시 열 경우 true, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


아카이브 내에 단일 항목을 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 엔트리의 이름. |
| source | java.io.InputStream | 항목에 대한 입력 스트림입니다. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


아카이브 내에 단일 항목을 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 엔트리의 이름. |
| path | java.lang.String | 압축할 파일의 경로입니다. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


아카이브 내에 단일 항목을 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 이름 | java.lang.String | 엔트리의 이름. |
| path | java.lang.String | 압축할 파일의 경로입니다. |
| openImmediately | boolean | 파일을 즉시 열 경우 true, 그렇지 않으면 아카이브 저장 시 파일을 엽니다. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


관리되지 않는 리소스를 해제하거나, 릴리스하거나, 재설정하는 애플리케이션 정의 작업을 수행합니다.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


제공된 디렉터리로 아카이브의 모든 파일을 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 추출된 파일을 배치할 디렉터리 경로입니다. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


아카이브를 구성하는 항목을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - 아카이브를 구성하는 항목.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


새로 구성된 항목에 사용되는 설정을 가져옵니다.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


아카이브가 솔리드 압축을 사용하는지 여부를 나타내는 값을 가져옵니다. 솔리드 모드에서는 모든 항목 데이터가 단일 스트림으로 압축되며 개별 항목 추출이 불가능합니다. 대신 [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--)를 사용하십시오.

**Returns:**
boolean - 아카이브가 솔리드 압축을 사용하는지 여부를 나타내는 값.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


제공된 스트림에 아카이브를 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 출력 | java.io.OutputStream | 대상 스트림. |

`output`은 쓰기 가능해야 합니다. LZ4와 같은 일부 압축 설정은 탐색 가능한 스트림도 필요합니다. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


제공된 대상 파일에 아카이브를 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationFileName | java.lang.String | 생성될 아카이브의 경로입니다. |

