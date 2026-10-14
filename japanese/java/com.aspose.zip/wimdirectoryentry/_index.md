---
title: "WimDirectoryEntry"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "wim アーカイブ内の単一ディレクトリを表します。"
type: docs
weight: 131
url: /ja/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

wim アーカイブ内の単一ディレクトリを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。 |
| [getAllEntries()](#getAllEntries--) | ディレクトリを構成するすべての [WimEntry](../../com.aspose.zip/wimentry) タイプのエントリを再帰的に取得します。 |
| [getDirectories()](#getDirectories--) | ディレクトリを構成する [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) タイプのエントリを取得します。 |
| [getFiles()](#getFiles--) | ディレクトリを構成する [WimFileEntry](../../com.aspose.zip/wimfileentry) タイプのエントリを取得します。 |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | ディレクトリを構成する [WimEntry](../../com.aspose.zip/wimentry) タイプのエントリを取得します。 |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


現在のディレクトリ内のすべてのファイルを、指定されたディレクトリへ抽出します。

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().extractToDirectory(\"C:\\\\extracted\");
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
