---
title: "WimEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "wim 이미지 내 단일 파일 또는 디렉터리를 나타냅니다."
type: docs
weight: 132
url: /ko/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

wim 이미지 내 단일 파일 또는 디렉터리를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | 파일 또는 디렉터리의 대체 데이터 스트림 이름을 가져옵니다. |
| [getArchive()](#getArchive--) | 항목이 속한 아카이브를 가져옵니다. |
| [getChangeTime()](#getChangeTime--) | 파일 또는 디렉터리가 마지막으로 변경된 시간을 가져옵니다. |
| [getCreationTime()](#getCreationTime--) | 파일 또는 디렉터리의 생성 시간을 가져옵니다. |
| [getFileAttributes()](#getFileAttributes--) | 파일 또는 디렉터리 속성을 가져옵니다. |
| [getFullPath()](#getFullPath--) | 이미지 내 항목의 전체 경로를 가져옵니다. |
| [getHardLink()](#getHardLink--) | 파일 또는 디렉터리의 하드링크 ID를 가져옵니다. |
| [getImage()](#getImage--) | 항목이 속한 이미지를 가져옵니다. |
| [getLastAccessTime()](#getLastAccessTime--) | 파일 또는 디렉터리의 마지막 접근 시간을 가져옵니다. |
| [getLastWriteTime()](#getLastWriteTime--) | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| [getName()](#getName--) | 이미지 내 항목의 이름을 가져옵니다. |
| [getParent()](#getParent--) | 항목이 속한 상위 디렉터리를 가져옵니다. |
| [getShortName()](#getShortName--) | 이미지 내 항목의 짧은 이름을 가져옵니다. |
| [hasHardLinks()](#hasHardLinks--) | 파일 또는 디렉터리가 다른 이름으로 알려져 있는지 여부를 가져옵니다. |
| [isDirectory()](#isDirectory--) | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [toString()](#toString--) | 인스턴스인 [WimEntry](../../com.aspose.zip/wimentry) 클래스의 문자열 표현을 반환합니다. |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


파일 또는 디렉터리의 대체 데이터 스트림 이름을 가져옵니다.

**Returns:**
java.lang.String[] - 파일 또는 디렉터리의 대체 데이터 스트림 이름
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


항목이 속한 아카이브를 가져옵니다.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


파일 또는 디렉터리가 마지막으로 변경된 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리가 마지막으로 변경된 시간
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


파일 또는 디렉터리의 생성 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리의 생성 시간
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


파일 또는 디렉터리 속성을 가져옵니다.

**Returns:**
int - 파일 또는 디렉터리 속성
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


이미지 내 항목의 전체 경로를 가져옵니다.

**Returns:**
java.lang.String - 이미지 내 항목의 전체 경로
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


파일 또는 디렉터리의 하드링크 ID를 가져옵니다.

**Returns:**
long - 파일 또는 디렉터리의 하드링크 ID
### getImage() {#getImage--}
```
public final WimImage getImage()
```


항목이 속한 이미지를 가져옵니다.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


파일 또는 디렉터리의 마지막 접근 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리의 마지막 접근 시간
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


파일 또는 디렉터리의 수정 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리의 수정 시간
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


파일 또는 디렉터리의 수정 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리의 수정 시간
### getName() {#getName--}
```
public final String getName()
```


이미지 내 항목의 이름을 가져옵니다.

**Returns:**
java.lang.String - 이미지 내 항목의 이름
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


항목이 속한 상위 디렉터리를 가져옵니다.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


이미지 내 항목의 짧은 이름을 가져옵니다.

**Returns:**
java.lang.String - 이미지 내 항목의 짧은 이름
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


파일 또는 디렉터리가 다른 이름으로 알려져 있는지 여부를 가져옵니다.

**Returns:**
boolean - 파일 또는 디렉터리가 다른 이름으로 알려져 있는지 여부
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 항목이 디렉터리를 나타내는지 여부를 나타내는 값
### toString() {#toString--}
```
public String toString()
```


인스턴스인 [WimEntry](../../com.aspose.zip/wimentry) 클래스의 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 이 객체의 문자열 표현
