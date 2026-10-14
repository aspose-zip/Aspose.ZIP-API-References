---
title: "SplitArchiveSaveOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para guardar un archivo ZIP de varios volúmenes."
type: docs
weight: 122
url: /es/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Opciones para guardar un archivo ZIP de varios volúmenes.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Instancia la configuración para guardar un archivo ZIP de varios volúmenes. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Obtiene el comentario opcional para el archivo Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Obtiene un valor que indica si las fuentes de las entradas deben cerrarse justo después de que una entrada haya sido comprimida. |
| [getEncoding()](#getEncoding--) | Obtiene la codificación para convertir nombres de archivo y otras cadenas a bytes. |
| [getEventsBag()](#getEventsBag--) | Obtiene el contenedor de eventos que se generan al guardar el archivo. |
| [getFileName()](#getFileName--) | Obtiene el nombre de los segmentos sin extensión. |
| [getSegmentSize()](#getSegmentSize--) | Obtiene el tamaño del segmento. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Establece el comentario opcional para el archivo Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Establece un valor que indica si las fuentes de las entradas deben cerrarse justo después de que una entrada haya sido comprimida. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Establece la codificación para convertir nombres de archivo y otras cadenas a bytes. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Establece el contenedor de eventos que se generan al guardar el archivo. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Instancia la configuración para guardar un archivo ZIP de varios volúmenes.

Algunos volúmenes pueden ser menores que `segmentSize`. En la mayoría de los casos, el último segmento será menor, pero rara vez los segmentos regulares podrían ser demasiado.

Los nombres de los archivos serán los siguientes: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | Nombre para los volúmenes. Puede ser con o sin la extensión .zip. |
| segmentSize | long | Tamaño del volumen. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Obtiene el comentario opcional para el archivo Zip.

**Returns:**
java.lang.String - comentario opcional para el archivo Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Obtiene un valor que indica si las fuentes de las entradas deben cerrarse justo después de que una entrada haya sido comprimida.

**Returns:**
boolean - un valor que indica si las fuentes de las entradas deben cerrarse justo después de que una entrada haya sido comprimida.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Obtiene la codificación para convertir nombres de archivo y otras cadenas a bytes.

Si no se establece, se utilizará la página de códigos 437.

**Returns:**
java.nio.charset.Charset - codificación para convertir nombres de archivo y otras cadenas a bytes.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Obtiene el contenedor de eventos que se generan al guardar el archivo.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtiene el nombre de los segmentos sin extensión.

**Returns:**
java.lang.String - el nombre de los segmentos sin extensión.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Obtiene el tamaño del segmento.

**Returns:**
long - el tamaño del segmento.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Establece el comentario opcional para el archivo Zip.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | comentario opcional para el archivo Zip. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Establece un valor que indica si las fuentes de las entradas deben cerrarse justo después de que una entrada haya sido comprimida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las fuentes de las entradas deben cerrarse justo después de que una entrada haya sido comprimida. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Establece la codificación para convertir nombres de archivo y otras cadenas a bytes.

Si no se establece, se utilizará la página de códigos 437.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.nio.charset.Charset | codificación para convertir nombres de archivo y otras cadenas a bytes. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Establece el contenedor de eventos que se generan al guardar el archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | contenedor de eventos que se generan al guardar el archivo. |

