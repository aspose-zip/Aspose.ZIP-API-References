---
title: "WimImage"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Wim arşivindeki tek bir görüntüyü temsil eder."
type: docs
weight: 134
url: /tr/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

Wim arşivindeki tek bir görüntüyü temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Görüntüdeki tüm dosyaları belirtilen dizine çıkarır. |
| [getAllEntries()](#getAllEntries--) | Görüntüyü oluşturan [WimEntry](../../com.aspose.zip/wimentry) türündeki girişleri özyinelemeli olarak alır. |
| [getEntry(String path)](#getEntry-java.lang.String-) | Verilen yol için [WimEntry](../../com.aspose.zip/wimentry) türündeki girişi alır. |
| [getParent()](#getParent--) | Görüntünün ait olduğu arşivi alır. |
| [getRootDirectory()](#getRootDirectory--) | Görüntünün kök dizin girişini alır. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Görüntüdeki tüm dosyaları belirtilen dizine çıkarır.

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
