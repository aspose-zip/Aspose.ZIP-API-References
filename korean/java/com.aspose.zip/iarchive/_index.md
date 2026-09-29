---
title: "IArchive"
second_title: "Aspose.ZIP for Java API 참조"
description: "이 인터페이스는 아카이브를 나타냅니다."
type: docs
weight: 161
url: /ko/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

이 인터페이스는 아카이브를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 제공된 디렉터리로 아카이브의 모든 파일을 추출합니다. |
| [getFileEntries()](#getFileEntries--) | 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다. |
| [getFormat()](#getFormat--) | 아카이브 형식을 가져옵니다. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


제공된 디렉터리로 아카이브의 모든 파일을 추출합니다.

디렉터리가 존재하지 않으면 생성됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| destinationDirectory | java.lang.String | 추출된 파일을 배치할 디렉터리 경로입니다. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목을 가져옵니다.

gzip, bzip2, lzip, lzma, lz4, xz, z와 같은 압축 전용 아카이브는 단일 레코드(아카이브 자체)로 구성됩니다.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - 아카이브를 구성하는 [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) 유형의 항목들.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


아카이브 형식을 가져옵니다.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
