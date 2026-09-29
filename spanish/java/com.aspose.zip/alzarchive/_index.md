---
title: "AlzArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un archivo ALZ."
type: docs
weight: 11
url: /es/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Representa un archivo ALZ. Utilice esta clase para inspeccionar y extraer archivos ALZ.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Inicializa un archivo ALZ a partir de un flujo. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Inicializa un archivo ALZ a partir de un flujo usando las opciones de carga suministradas. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Inicializa un archivo ALZ a partir de una ruta de archivo. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Inicializa un archivo ALZ a partir de una ruta de archivo usando las opciones de carga suministradas. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | Libera los recursos mantenidos por este archivo. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos y directorios al directorio proporcionado. |
| [getEntries()](#getEntries--) | Obtiene las entradas que constituyen este archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas a través de la interfaz común de archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Inicializa un archivo ALZ a partir de un flujo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Flujo de archivo ALZ; debe soportar lectura y búsqueda |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Inicializa un archivo ALZ a partir de un flujo usando las opciones de carga suministradas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | Flujo de archivo ALZ; debe soportar lectura y búsqueda |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opciones usadas para cargar el archivo |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Inicializa un archivo ALZ a partir de una ruta de archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | ruta a un archivo ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Inicializa un archivo ALZ a partir de una ruta de archivo usando las opciones de carga suministradas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | ruta a un archivo ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opciones usadas para cargar el archivo |

### close() {#close--}
```
public void close()
```


Libera los recursos mantenidos por este archivo.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrae todos los archivos y directorios al directorio proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | java.lang.String | directorio de destino; se crea cuando es necesario |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Obtiene las entradas que constituyen este archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - lista inmutable de entradas ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas a través de la interfaz común de archivo.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del archivo
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
