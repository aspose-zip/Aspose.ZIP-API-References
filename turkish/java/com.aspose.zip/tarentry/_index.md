---
title: "TarEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Tar arşivindeki tek bir dosyayı temsil eder."
type: docs
weight: 126
url: /tr/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Tar arşivindeki tek bir dosyayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getModificationTime()](#getModificationTime--) | Dosyanın veya dizinin değiştirilme zamanını alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
| [isDirectory()](#isDirectory--) | Girdinin bir dizin olup olmadığını gösteren değeri alır. |
| [open()](#open--) | Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar. |
| [setName(String value)](#setName-java.lang.String-) | Arşiv içindeki girdinin adını ayarlar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

Tar arşivinden bir girdiyi çıkar.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

**Returns:**
java.io.File - çıkarılan dosyanın dosya bilgisi
### getLength() {#getLength--}
```
public final Long getLength()
```


Girdinin uzunluğunu bayt cinsinden alır.

**Returns:**
java.lang.Long - girişin bayt cinsinden uzunluğu
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Dosyanın veya dizinin değiştirilme zamanını alır.

**Returns:**
java.util.Date - dosyanın veya dizinin değiştirilme zamanı.
### getName() {#getName--}
```
public final String getName()
```


Arşiv içindeki girdinin adını alır.

**Returns:**
java.lang.String - arşiv içindeki girdinin adı
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Orijinal dosyanın boyutunu alır.

`Length`([getLength](../../com.aspose.zip/tarentry\\#getLength--)) ile aynı değere sahiptir

**Returns:**
long - orijinal dosyanın boyutu.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Girdinin bir dizin olup olmadığını gösteren değeri alır.

**Returns:**
boolean - girişin bir dizin olup olmadığını gösteren değer
### open() {#open--}
```
public final InputStream open()
```


Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar.


Kullanım:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

