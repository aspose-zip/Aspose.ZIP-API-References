---
title: "ComHelper"
second_title: "Aspose.ZIP for Java API Referansı"
description: "COM istemcilerinin arşivleri Aspose.Zip'e yüklemesi için yöntemler sağlar."
type: docs
weight: 55
url: /tr/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

COM istemcilerinin arşivleri Aspose.Zip'e yüklemesi için yöntemler sağlar.

ComHelper sınıfını bir dosyadan veya akıştan arşiv yüklemek için kullanın. Belirli sınıflar yeni bir arşiv oluşturmak için varsayılan yapıcıyı sağlar ve ayrıca bir dosyadan veya akıştan arşiv yüklemek için aşırı yüklenmiş yapıcılar sunar. .NET uygulamasında Aspose.Zip kullanıyorsanız, tüm arşiv yapıcılarını doğrudan kullanabilirsiniz, ancak bir COM uygulamasında Aspose.Zip kullanıyorsanız yalnızca varsayılan arşiv yapıcısı mevcuttur.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ComHelper()](#ComHelper--) | Bu sınıfın yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Bir COM uygulamasının bir akıştan bzip2 arşivi yüklemesine izin verir. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Bir COM uygulamasının bir dosyadan bzip2 arşivi yüklemesine izin verir. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Bir COM uygulamasının bir gzip arşivini bir akıştan yüklemesine izin verir. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Bir COM uygulamasının bir gzip arşivini bir dosyadan yüklemesine izin verir. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Bir COM uygulamasının bir rar arşivini bir akıştan yüklemesine izin verir. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Bir COM uygulamasının bir rar arşivini bir dosyadan yüklemesine izin verir. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Bir COM uygulamasının bir ZIP arşivini bir akıştan yüklemesine izin verir. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Bir COM uygulamasının bir ZIP arşivini bir dosyadan yüklemesine izin verir. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Bu sınıfın yeni bir örneğini başlatır.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Bir COM uygulamasının bir akıştan bzip2 arşivi yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Yüklenecek arşivi içeren bir .NET akış nesnesi. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Bir COM uygulamasının bir dosyadan bzip2 arşivi yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Yüklenecek arşivin dosya adı. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Bir COM uygulamasının bir gzip arşivini bir akıştan yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Yüklenecek arşivi içeren bir .NET akış nesnesi. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Bir COM uygulamasının bir gzip arşivini bir dosyadan yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Yüklenecek arşivin dosya adı. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Bir COM uygulamasının bir rar arşivini bir akıştan yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Yüklenecek arşivi içeren bir .NET akış nesnesi. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Bir COM uygulamasının bir rar arşivini bir dosyadan yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Yüklenecek arşivin dosya adı. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Bir COM uygulamasının bir ZIP arşivini bir akıştan yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | java.io.InputStream | Yüklenecek arşivi içeren bir .NET akış nesnesi. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Bir COM uygulamasının bir ZIP arşivini bir dosyadan yüklemesine izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Yüklenecek arşivin dosya adı. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
