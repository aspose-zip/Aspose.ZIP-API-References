---
title: "ArchiveInstanceInfo"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa información sobre la instancia del archivo."
type: docs
weight: 34
url: /es/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Representa información sobre la instancia del archivo.
## Métodos

| Método | Descripción |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Obtiene un valor que indica si los nombres de las entradas (archivos) del archivo están encriptados. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Obtiene información del formato del archivo. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Obtiene información del formato del archivo. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Obtiene información de la instancia del archivo. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Obtiene información de la instancia del archivo. |
| [getFormatInfo()](#getFormatInfo--) | Obtiene la información del formato del archivo. |
| [isContentEncrypted()](#isContentEncrypted--) | Obtiene un valor que indica si el contenido del archivo está cifrado. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Obtiene un valor que indica si los nombres de las entradas (archivos) del archivo están encriptados.

**Returns:**
boolean - un valor que indica si los nombres de las entradas (archivos) del archivo están cifrados.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Obtiene información del formato del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo del archivo del archivo. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Obtiene información del formato del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre de archivo del archivo del archivo. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Obtiene información de la instancia del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.InputStream | El flujo del archivo del archivo. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Obtiene información de la instancia del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | El nombre de archivo del archivo del archivo. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Obtiene la información del formato del archivo.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Obtiene un valor que indica si el contenido del archivo está cifrado.

**Returns:**
boolean - un valor que indica si el contenido del archivo está cifrado.
