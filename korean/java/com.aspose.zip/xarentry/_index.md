---
title: "XarEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "xar 아카이브 내 단일 항목을 나타냅니다."
type: docs
weight: 140
url: /ko/java/com.aspose.zip/xarentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class XarEntry
```

xar 아카이브 내 단일 항목을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | 파일 또는 디렉터리의 생성 시간을 가져옵니다. |
| [getFullPath()](#getFullPath--) | 아카이브 내 항목의 전체 경로를 가져옵니다. |
| [getLastAccessTime()](#getLastAccessTime--) | 파일 또는 디렉터리의 마지막 접근 시간을 가져옵니다. |
| [getLastWriteTime()](#getLastWriteTime--) | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| [getModificationTime()](#getModificationTime--) | 파일 또는 디렉터리의 수정 시간을 가져옵니다. |
| [getName()](#getName--) | 아카이브 내 항목의 이름을 가져옵니다. |
| [getParent()](#getParent--) | 항목이 속한 상위 디렉터리를 가져옵니다. |
| [isDirectory()](#isDirectory--) | 항목이 디렉터리를 나타내는지 여부를 나타내는 값을 가져옵니다. |
| [toString()](#toString--) | 인스턴스인 [XarEntry](../../com.aspose.zip/xarentry) 클래스의 문자열 표현을 반환합니다. |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


파일 또는 디렉터리의 생성 시간을 가져옵니다.

**Returns:**
java.util.Date - 파일 또는 디렉터리의 생성 시간
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


아카이브 내 항목의 전체 경로를 가져옵니다.

**Returns:**
java.lang.String - 아카이브 내 항목의 전체 경로
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


아카이브 내 항목의 이름을 가져옵니다.

**Returns:**
java.lang.String - 아카이브 내 항목의 이름
### getParent() {#getParent--}
```
public final XarDirectoryEntry getParent()
```


항목이 속한 상위 디렉터리를 가져옵니다.

**Returns:**
[XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) - the parent directory the entry belongs to
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


인스턴스인 [XarEntry](../../com.aspose.zip/xarentry) 클래스의 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 이 객체의 문자열 표현
