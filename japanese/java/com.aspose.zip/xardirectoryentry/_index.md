---
title: "XarDirectoryEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "xar アーカイブ内のディレクトリエントリを表します。"
type: docs
weight: 139
url: /ja/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object、[com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

xar アーカイブ内のディレクトリエントリを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。 |
| [getAllEntries()](#getAllEntries--) | ディレクトリを構成するすべての [XarEntry](../../com.aspose.zip/xarentry) タイプのエントリを再帰的に取得します。 |
| [getDirectories()](#getDirectories--) | ディレクトリを構成する [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) タイプのエントリを取得します。 |
| [getFiles()](#getFiles--) | ディレクトリを構成する [XarFileEntry](../../com.aspose.zip/xarfileentry) タイプのエントリを取得します。 |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | ディレクトリを構成する [XarEntry](../../com.aspose.zip/xarentry) タイプのエントリを取得します。 |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。

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
