---
title: "ArjEntryPlain"
second_title: "Aspose.ZIP for Java API Referansı"
description: "ARJ arşivi içinde tek bir dosyayı temsil eder."
type: docs
weight: 38
url: /tr/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

ARJ arşivi içinde tek bir dosyayı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | ARJ arşiv girdisini bir dosyaya çıkarır. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getCompressedSize()](#getCompressedSize--) | Sıkıştırılmış dosyanın boyutunu alır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Arşiv içindeki girdinin adını alır. |
| [getUncompressedSize()](#getUncompressedSize--) | Orijinal dosyanın boyutunu alır. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


ARJ arşiv girdisini bir dosyaya çıkarır.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

**Returns:**
java.io.File - birleştirilmiş dosyanın dosya bilgisi
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Sıkıştırılmış dosyanın boyutunu alır.

**Returns:**
long - sıkıştırılmış dosyanın boyutu
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
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Orijinal dosyanın boyutunu alır.

**Returns:**
long - orijinal dosyanın boyutu
