---
title: "AlzArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "ALZ 아카이브 파일을 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

ALZ 아카이브 파일을 나타냅니다. 이 클래스를 사용하여 ALZ 아카이브를 검사하고 추출합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | 스트림에서 ALZ 아카이브를 초기화합니다. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | 제공된 로드 옵션을 사용하여 스트림에서 ALZ 아카이브를 초기화합니다. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | 파일 경로에서 ALZ 아카이브를 초기화합니다. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | 제공된 로드 옵션을 사용하여 파일 경로에서 ALZ 아카이브를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | 이 아카이브가 보유한 리소스를 해제합니다. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 모든 파일 및 디렉터리를 추출합니다. |
| [getEntries()](#getEntries--) | 이 아카이브를 구성하는 항목을 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | 공통 아카이브 인터페이스를 통해 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


스트림에서 ALZ 아카이브를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | ALZ 아카이브 스트림; 읽기 및 탐색을 지원해야 합니다 |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


제공된 로드 옵션을 사용하여 스트림에서 ALZ 아카이브를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | ALZ 아카이브 스트림; 읽기 및 탐색을 지원해야 합니다 |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | 아카이브를 로드하는 데 사용되는 옵션 |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


파일 경로에서 ALZ 아카이브를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | ALZ 아카이브 경로 |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


제공된 로드 옵션을 사용하여 파일 경로에서 ALZ 아카이브를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | ALZ 아카이브 경로 |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | 아카이브를 로드하는 데 사용되는 옵션 |

### close() {#close--}
```
public void close()
```


이 아카이브가 보유한 리소스를 해제합니다.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


제공된 디렉터리로 모든 파일 및 디렉터리를 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 대상 디렉터리; 필요할 때 생성됩니다 |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


이 아카이브를 구성하는 항목을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - ALZ 항목의 불변 리스트
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


공통 아카이브 인터페이스를 통해 항목을 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 아카이브 항목
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
