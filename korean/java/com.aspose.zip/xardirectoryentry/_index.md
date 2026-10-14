---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP for Java API 참조"
description: "xar 아카이브 내 디렉터리 항목을 나타냅니다."
type: docs
weight: 139
url: /ko/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

xar 아카이브 내 디렉터리 항목을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 현재 디렉터리의 모든 파일을 제공된 디렉터리로 추출합니다. |
| [getAllEntries()](#getAllEntries--) | 디렉터리를 재귀적으로 구성하는 [XarEntry](../../com.aspose.zip/xarentry) 유형의 모든 항목을 가져옵니다. |
| [getDirectories()](#getDirectories--) | 디렉터리를 구성하는 [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) 유형의 항목을 가져옵니다. |
| [getFiles()](#getFiles--) | 디렉터리를 구성하는 [XarFileEntry](../../com.aspose.zip/xarfileentry) 유형의 항목을 가져옵니다. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | 디렉터리를 구성하는 [XarEntry](../../com.aspose.zip/xarentry) 유형의 항목을 가져옵니다. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


현재 디렉터리의 모든 파일을 제공된 디렉터리로 추출합니다.

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
((XarDirectoryEntry)archive.getEntries().get(0)).extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<XarEntry> getAllEntries()
```


Gets all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final Iterable<XarDirectoryEntry> getDirectories()
```


Gets entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarDirectoryEntry&gt; - entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final Iterable<XarFileEntry> getFiles()
```


Gets entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarFileEntry&gt; - entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<XarEntry> getFilesAndDirectories()
```


Gets entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory
