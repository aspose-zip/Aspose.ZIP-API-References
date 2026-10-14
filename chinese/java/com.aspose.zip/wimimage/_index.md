---
title: "WimImage"
second_title: "Aspose.ZIP for Java API 参考"
description: "表示 wim 存档中的单个镜像。"
type: docs
weight: 134
url: /zh/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

表示 wim 存档中的单个镜像。
## 方法

| 方法 | 描述 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 将映像中的所有文件提取到提供的目录。 |
| [getAllEntries()](#getAllEntries--) | 获取构成映像的 [WimEntry](../../com.aspose.zip/wimentry) 类型的条目，递归地。 |
| [getEntry(String path)](#getEntry-java.lang.String-) | 获取给定路径的 [WimEntry](../../com.aspose.zip/wimentry) 类型的条目。 |
| [getParent()](#getParent--) | 获取映像所属的归档。 |
| [getRootDirectory()](#getRootDirectory--) | 获取映像的根目录条目。 |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


将映像中的所有文件提取到提供的目录。

```

``````

try (WimArchive archive = new WimArchive(\"install.wim\")) {
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
