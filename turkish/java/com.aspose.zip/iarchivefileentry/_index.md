---
title: "IArchiveFileEntry"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bu arayüz bir arşiv dosyası girişini temsil eder."
type: docs
weight: 162
url: /tr/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Bu arayüz bir arşiv dosyası girişini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Girdiyi sağlanan akıma çıkarır. |
| [extract(String path)](#extract-java.lang.String-) | Girdiyi sağlanan yola göre dosya sistemine çıkarır. |
| [getLength()](#getLength--) | Girdinin uzunluğunu bayt cinsinden alır. |
| [getName()](#getName--) | Girişin adını alır. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Girdiyi sağlanan akıma çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hedef | java.io.OutputStream | hedef akış. Yazılabilir olmalıdır |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Girdiyi sağlanan yola göre dosya sistemine çıkarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| path | java.lang.String | hedef dosyanın yolu. Dosya zaten mevcutsa, üzerine yazılacaktır. |

**Returns:**
java.io.File - çıkarılan veriyi içeren java.io.File örneği
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Girdinin uzunluğunu bayt cinsinden alır.

**Returns:**
java.lang.Long - girişin bayt cinsinden uzunluğu
### getName() {#getName--}
```
public abstract String getName()
```


Girişin adını alır.

Sıkıştırma amaçlı arşivler, örneğin gzip, bzip2, lzip, lzma, xz, z, başlıklarda başka bir ad bulunmadığı sürece "File.bin" adını alır.

**Returns:**
java.lang.String - girişin adı
