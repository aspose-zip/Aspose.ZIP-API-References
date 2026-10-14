---
title: "CpioEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "cpio arşivi içinde tek bir dosyayı temsil eder."
type: docs
weight: 58
url: /tr/java/com.aspose.zip/cpioentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CpioEntry implements IArchiveFileEntry
```

cpio arşivi içinde tek bir dosyayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getLastWriteTimeUtc()](#getLastWriteTimeUtc--) | Son yazma zamanını alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getParent()](#getParent--) | Girdinin ait olduğu arşivi alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [open()](#open--) | Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar. |
| [toString()](#toString--) | [CpioEntry](../../com.aspose.zip/cpioentry) sınıfının örneğinin dize temsilini döndürür. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

cpio arşivinden bir girdi çıkar.

```

``````

try (CpioArchive archive = new CpioArchive("archive.cpio")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CpioArchive archive = new CpioArchive("archive.cpio")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

**Returns:**
java.io.File - çıkarılan dosyanın dosya bilgisi
### getLastWriteTimeUtc() {#getLastWriteTimeUtc--}
```
public final Date getLastWriteTimeUtc()
```


Son yazma zamanını alır.

**Returns:**
java.util.Date - son yazma zamanı
### getLength() {#getLength--}
```
public final Long getLength()
```


Girdinin uzunluğunu bayt cinsinden alır.

**Returns:**
java.lang.Long - girişin bayt cinsinden uzunluğu
### getName() {#getName--}
```
public final String getName()
```


Arşiv içindeki girdinin adını alır.

**Returns:**
java.lang.String - arşiv içindeki girdinin adı
### getParent() {#getParent--}
```
public final CpioArchive getParent()
```


Girdinin ait olduğu arşivi alır.

**Returns:**
[CpioArchive](../../com.aspose.zip/cpioarchive) - the archive the entry belongs to
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Girdinin bir dizin olup olmadığını gösteren değeri alır.

**Returns:**
boolean - bir değer, girdinin bir dizin olup olmadığını gösterir.
### open() {#open--}
```
public final InputStream open()
```


Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar.

Kullanım:

```

``````

CpioArchive archive = new CpioArchive("archive.cpio");
CpioEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CpioEntry](../../com.aspose.zip/cpioentry) class.

**Returns:**
java.lang.String - string representation of this object.
