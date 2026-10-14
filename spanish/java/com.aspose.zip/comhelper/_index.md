---
title: "ComHelper"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Proporciona métodos para que los clientes COM carguen archivos en Aspose.Zip."
type: docs
weight: 55
url: /es/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Proporciona métodos para que los clientes COM carguen archivos en Aspose.Zip.

Utilice la clase ComHelper para cargar un archivo desde un archivo o flujo. Las clases particulares proporcionan un constructor predeterminado para crear un nuevo archivo y también proporcionan constructores sobrecargados para cargar un archivo desde un archivo o flujo. Si está utilizando Aspose.Zip desde una aplicación .NET, puede utilizar todos los constructores de archivo directamente, pero si está utilizando Aspose.Zip desde una aplicación COM, solo está disponible el constructor predeterminado del archivo.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ComHelper()](#ComHelper--) | Inicializa una nueva instancia de esta clase. |
## Métodos

| Método | Descripción |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Permite a una aplicación COM cargar un archivo bzip2 desde un flujo. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Permite a una aplicación COM cargar un archivo bzip2 desde un archivo. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Permite a una aplicación COM cargar un archivo gzip desde un flujo. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Permite a una aplicación COM cargar un archivo gzip desde un archivo. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Permite a una aplicación COM cargar un archivo rar desde un flujo. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Permite a una aplicación COM cargar un archivo rar desde un archivo. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Permite a una aplicación COM cargar un archivo ZIP desde un flujo. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Permite a una aplicación COM cargar un archivo ZIP desde un archivo. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Inicializa una nueva instancia de esta clase.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Permite a una aplicación COM cargar un archivo bzip2 desde un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Un objeto de flujo .NET que contiene el archivo a cargar. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Permite a una aplicación COM cargar un archivo bzip2 desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | Nombre del archivo del archivo a cargar. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Permite a una aplicación COM cargar un archivo gzip desde un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Un objeto de flujo .NET que contiene el archivo a cargar. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Permite a una aplicación COM cargar un archivo gzip desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | Nombre del archivo del archivo a cargar. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Permite a una aplicación COM cargar un archivo rar desde un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Un objeto de flujo .NET que contiene el archivo a cargar. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Permite a una aplicación COM cargar un archivo rar desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | Nombre del archivo del archivo a cargar. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Permite a una aplicación COM cargar un archivo ZIP desde un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Un objeto de flujo .NET que contiene el archivo a cargar. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Permite a una aplicación COM cargar un archivo ZIP desde un archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | Nombre del archivo del archivo a cargar. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
