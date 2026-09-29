---
title: "WimImage"
second_title: "Aspose.ZIP for Java API 참조"
description: "wim 아카이브 내 단일 이미지를 나타냅니다."
type: docs
weight: 134
url: /ko/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

wim 아카이브 내 단일 이미지를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | 이미지의 모든 파일을 제공된 디렉터리로 추출합니다. |
| [getAllEntries()](#getAllEntries--) | 이미지를 구성하는 [WimEntry](../../com.aspose.zip/wimentry) 유형의 항목을 재귀적으로 가져옵니다. |
| [getEntry(String path)](#getEntry-java.lang.String-) | 주어진 경로에 대한 [WimEntry](../../com.aspose.zip/wimentry) 유형의 항목을 가져옵니다. |
| [getParent()](#getParent--) | 이미지가 속한 아카이브를 가져옵니다. |
| [getRootDirectory()](#getRootDirectory--) | 이미지의 루트 디렉터리 항목을 가져옵니다. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


이미지의 모든 파일을 제공된 디렉터리로 추출합니다.

```

``````

try (WimArchive archive = new WimArchive("install.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
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
