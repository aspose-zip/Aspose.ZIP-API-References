---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 xar 存档中的目录条目。"
type: docs
weight: 139
url: /zh/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

表示 xar 存档中的目录条目。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将当前目录中的所有文件提取到提供的目录。 |
| [getAllEntries()](#getAllEntries--) | 递归获取目录中所有 [XarEntry](../../com.aspose.zip/xarentry) 类型的条目。 |
| [getDirectories()](#getDirectories--) | 获取构成目录的 [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) 类型的条目。 |
| [getFiles()](#getFiles--) | 获取构成目录的 [XarFileEntry](../../com.aspose.zip/xarfileentry) 类型的条目。 |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | 获取构成目录的 [XarEntry](../../com.aspose.zip/xarentry) 类型的条目。 |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将当前目录中的所有文件提取到提供的目录。

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
