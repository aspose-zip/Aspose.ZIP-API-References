---
title: "CabEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "cab arşivi içinde tek bir dosyayı temsil eder."
type: docs
weight: 46
url: /tr/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

cab arşivi içinde tek bir dosyayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getModificationTime()](#getModificationTime--) | Son değiştirilme tarih ve saatini alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [open()](#open--) | Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar. |
| [toString()](#toString--) | Bir [CabEntry](../../com.aspose.zip/cabentry) sınıfı örneğinin dize temsili döndürür. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

CAB arşivinden bir giriş çıkar.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
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

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

**Returns:**
java.io.File - birleştirilmiş dosyanın dosya bilgisi
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


Son değiştirilme tarih ve saatini alır.

**Returns:**
java.util.Date - son değiştirilme tarihi ve saati.
### getName() {#getName--}
```
public final String getName()
```


Arşiv içindeki girdinin adını alır.

**Returns:**
java.lang.String - arşiv içindeki girdinin adı
### open() {#open--}
```
public final InputStream open()
```


Girdiyi çıkarmak için açar ve giriş içeriğiyle bir akış sağlar.

Kullanım:

```

``````

CabArchive archive = new CabArchive("archive.cab");
CabEntry entry = archive.getEntries().get(0);
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


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
