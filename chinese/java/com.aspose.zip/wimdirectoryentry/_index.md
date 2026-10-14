---
title: "WimDirectoryEntry"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 wim 存档中的单个目录。"
type: docs
weight: 131
url: /zh/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

表示 wim 存档中的单个目录。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将当前目录中的所有文件提取到提供的目录。 |
| [getAllEntries()](#getAllEntries--) | 获取目录中递归构成的所有 [WimEntry](../../com.aspose.zip/wimentry) 类型的条目。 |
| [getDirectories()](#getDirectories--) | 获取构成目录的 [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) 类型的条目。 |
| [getFiles()](#getFiles--) | 获取构成目录的 [WimFileEntry](../../com.aspose.zip/wimfileentry) 类型的条目。 |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | 获取构成目录的 [WimEntry](../../com.aspose.zip/wimentry) 类型的条目。 |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将当前目录中的所有文件提取到提供的目录。

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<WimEntry> getAllEntries()
```


Gets all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final List<WimDirectoryEntry> getDirectories()
```


Gets entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimDirectoryEntry&gt; - entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final List<WimFileEntry> getFiles()
```


Gets entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimFileEntry&gt; - entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<WimEntry> getFilesAndDirectories()
```


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory
