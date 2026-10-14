---
title: "WimArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 클래스는 wim 아카이브 파일을 나타냅니다."
type: docs
weight: 130
url: /ko/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

이 클래스는 wim 아카이브 파일을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | 새로운 [WimArchive](../../com.aspose.zip/wimarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | 새로운 [WimArchive](../../com.aspose.zip/wimarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | 새로운 [WimArchive](../../com.aspose.zip/wimarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | 새로운 [WimArchive](../../com.aspose.zip/wimarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 아카이브를 경로에 따라 파일로 추출합니다. |
| [getBootImageIndex()](#getBootImageIndex--) | 부팅 가능한 이미지의 (0부터 시작하는) 인덱스를 가져옵니다. |
| [getEntries()](#getEntries--) | 아카이브를 구성하는 [WimEntry](../../com.aspose.zip/wimentry) 유형의 항목을 가져옵니다. |
| [getFileEntries()](#getFileEntries--) | wim 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFileFormatVersion()](#getFileFormatVersion--) | 파일 형식의 버전을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
| [getGuid()](#getGuid--) | 아카이브의 식별 UUID를 가져옵니다. |
| [getImages()](#getImages--) | 아카이브를 구성하는 [WimImage](../../com.aspose.zip/wimimage) 유형의 항목을 가져옵니다. |
| [getManifest()](#getManifest--) | 파일 및 포함된 이미지를 설명하는 내장 매니페스트를 가져옵니다. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


새로운 [WimArchive](../../com.aspose.zip/wimarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

이 생성자는 어떤 항목도 풀어내지 않습니다. 풀어내기 위해서는 [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sourceStream | java.io.InputStream | 아카이브의 소스 |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


새로운 [WimArchive](../../com.aspose.zip/wimarchive) 클래스 인스턴스를 초기화하고 아카이브에서 추출할 수 있는 항목 목록을 구성합니다.

다음 예제는 모든 항목을 디렉터리로 추출하는 방법을 보여줍니다.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

이 생성자는 어떤 항목도 풀어내지 않습니다. 풀어내기 위해서는 [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) 메서드를 참조하십시오.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| path | java.lang.String | 아카이브 파일의 경로 |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | 기존 아카이브를 로드하기 위한 옵션입니다. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


아카이브를 경로에 따라 파일로 추출합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 추출된 파일을 배치할 디렉터리 경로 |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


부팅 가능한 이미지의 (0부터 시작하는) 인덱스를 가져옵니다.

**Returns:**
int - 부팅 가능한 이미지의 (0부터 시작하는) 인덱스
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


아카이브를 구성하는 [WimEntry](../../com.aspose.zip/wimentry) 유형의 항목을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - 아카이브를 구성하는 항목
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


wim 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - wim 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


파일 형식의 버전을 가져옵니다.

**Returns:**
int - 파일 형식의 버전
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


아카이브의 식별 UUID를 가져옵니다.

**Returns:**
java.util.UUID - 아카이브를 식별하는 UUID
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


아카이브를 구성하는 [WimImage](../../com.aspose.zip/wimimage) 유형의 항목을 가져옵니다.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - 아카이브를 구성하는 [WimImage](../../com.aspose.zip/wimimage) 유형의 항목
### getManifest() {#getManifest--}
```
public final String getManifest()
```


파일 및 포함된 이미지를 설명하는 내장 매니페스트를 가져옵니다.

**Returns:**
java.lang.String - 파일 및 포함된 이미지를 설명하는 내장 매니페스트
