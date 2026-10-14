---
title: "ComHelper"
second_title: "Справочник API Aspose.ZIP для Java"
description: "Предоставляет методы для COM‑клиентов для загрузки архивов в Aspose.Zip."
type: docs
weight: 55
url: /ru/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Предоставляет методы для COM‑клиентов для загрузки архивов в Aspose.Zip.

Используйте класс ComHelper для загрузки архива из файла или потока. Конкретные классы предоставляют конструктор по умолчанию для создания нового архива, а также перегруженные конструкторы для загрузки архива из файла или потока. Если вы используете Aspose.Zip в приложении .NET, вы можете напрямую использовать все конструкторы архива, но если вы используете Aspose.Zip в COM‑приложении, доступен только конструктор архива по умолчанию.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [ComHelper()](#ComHelper--) | Инициализирует новый экземпляр этого класса. |
## Методы

| Метод | Описание |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Позволяет COM‑приложению загрузить архив bzip2 из потока. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Позволяет COM‑приложению загрузить архив bzip2 из файла. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Позволяет COM‑приложению загрузить архив gzip из потока. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Позволяет COM‑приложению загрузить архив gzip из файла. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Позволяет COM‑приложению загрузить архив rar из потока. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Позволяет COM‑приложению загрузить архив rar из файла. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Позволяет COM‑приложению загрузить архив ZIP из потока. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Позволяет COM‑приложению загрузить архив ZIP из файла. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Инициализирует новый экземпляр этого класса.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Позволяет COM‑приложению загрузить архив bzip2 из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Объект потока .NET, содержащий архив для загрузки. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Позволяет COM‑приложению загрузить архив bzip2 из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива для загрузки. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Позволяет COM‑приложению загрузить архив gzip из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Объект потока .NET, содержащий архив для загрузки. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Позволяет COM‑приложению загрузить архив gzip из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива для загрузки. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Позволяет COM‑приложению загрузить архив rar из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Объект потока .NET, содержащий архив для загрузки. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Позволяет COM‑приложению загрузить архив rar из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива для загрузки. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Позволяет COM‑приложению загрузить архив ZIP из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Объект потока .NET, содержащий архив для загрузки. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Позволяет COM‑приложению загрузить архив ZIP из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Имя файла архива для загрузки. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
