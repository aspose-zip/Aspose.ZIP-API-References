---
title: "WimDirectoryEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Wim arşivindeki tek bir dizini temsil eder."
type: docs
weight: 131
url: /tr/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

Wim arşivindeki tek bir dizini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Mevcut dizindeki tüm dosyaları belirtilen dizine çıkarır. |
| [getAllEntries()](#getAllEntries--) | Dizini yinelemeli olarak oluşturan [WimEntry](../../com.aspose.zip/wimentry) tipindeki tüm girdileri alır. |
| [getDirectories()](#getDirectories--) | Dizini oluşturan [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) tipindeki girdileri alır. |
| [getFiles()](#getFiles--) | Dizini oluşturan [WimFileEntry](../../com.aspose.zip/wimfileentry) tipindeki girdileri alır. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Dizini oluşturan [WimEntry](../../com.aspose.zip/wimentry) tipindeki girdileri alır. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Mevcut dizindeki tüm dosyaları belirtilen dizine çıkarır.

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
