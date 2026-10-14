---
title: "WimImage"
second_title: "Aspose.ZIP for Java API リファレンス"
description: "wim アーカイブ内の単一イメージを表します。"
type: docs
weight: 134
url: /ja/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

wim アーカイブ内の単一イメージを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | イメージ内のすべてのファイルを指定されたディレクトリに抽出します。 |
| [getAllEntries()](#getAllEntries--) | イメージを構成する [WimEntry](../../com.aspose.zip/wimentry) 型のエントリを再帰的に取得します。 |
| [getEntry(String path)](#getEntry-java.lang.String-) | 指定されたパスに対する [WimEntry](../../com.aspose.zip/wimentry) 型のエントリを取得します。 |
| [getParent()](#getParent--) | イメージが属するアーカイブを取得します。 |
| [getRootDirectory()](#getRootDirectory--) | イメージのルートディレクトリエントリを取得します。 |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


イメージ内のすべてのファイルを指定されたディレクトリに抽出します。

```

``````

try (WimArchive archive = new WimArchive("install.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
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


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the image recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the image recursively
### getEntry(String path) {#getEntry-java.lang.String-}
```
public final WimEntry getEntry(String path)
```


Gets the entry of [WimEntry](../../com.aspose.zip/wimentry) type for a given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of file or directory |

**Returns:**
[WimEntry](../../com.aspose.zip/wimentry) - the entry of [WimEntry](../../com.aspose.zip/wimentry) type
### getParent() {#getParent--}
```
public final WimArchive getParent()
```


Gets the archive the image belongs to.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the image belongs to
### getRootDirectory() {#getRootDirectory--}
```
public final WimDirectoryEntry getRootDirectory()
```


Gets the root directory entry of the image.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the root directory entry of the image
