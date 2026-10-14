---
title: "WimEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo o directorio dentro de la imagen wim."
type: docs
weight: 132
url: /es/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Representa un solo archivo o directorio dentro de la imagen wim.
## Métodos

| Método | Descripción |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Obtiene los nombres de los flujos de datos alternativos para el archivo o directorio. |
| [getArchive()](#getArchive--) | Obtiene el archivo al que pertenece la entrada. |
| [getChangeTime()](#getChangeTime--) | Obtiene la última vez que el archivo o directorio fue modificado. |
| [getCreationTime()](#getCreationTime--) | Obtiene la hora de creación del archivo o directorio. |
| [getFileAttributes()](#getFileAttributes--) | Obtiene los atributos del archivo o directorio. |
| [getFullPath()](#getFullPath--) | Obtiene la ruta completa de la entrada dentro de la imagen. |
| [getHardLink()](#getHardLink--) | Obtiene el ID del enlace duro del archivo o directorio. |
| [getImage()](#getImage--) | Obtiene la imagen a la que pertenece la entrada. |
| [getLastAccessTime()](#getLastAccessTime--) | Obtiene la última hora de acceso del archivo o directorio. |
| [getLastWriteTime()](#getLastWriteTime--) | Obtiene la hora de modificación del archivo o directorio. |
| [getModificationTime()](#getModificationTime--) | Obtiene la hora de modificación del archivo o directorio. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro de la imagen. |
| [getParent()](#getParent--) | Obtiene el directorio padre al que pertenece la entrada. |
| [getShortName()](#getShortName--) | Obtiene el nombre corto de la entrada dentro de la imagen. |
| [hasHardLinks()](#hasHardLinks--) | Obtiene si el archivo o directorio es conocido por otros nombres. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada representa un directorio. |
| [toString()](#toString--) | Devuelve la representación en cadena de la instancia de la clase [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Obtiene los nombres de los flujos de datos alternativos para el archivo o directorio.

**Returns:**
java.lang.String[] - los nombres de los flujos de datos alternativos para el archivo o directorio
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Obtiene el archivo al que pertenece la entrada.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Obtiene la última vez que el archivo o directorio fue modificado.

**Returns:**
java.util.Date - la última vez que el archivo o directorio fue modificado
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtiene la hora de creación del archivo o directorio.

**Returns:**
java.util.Date - la hora de creación del archivo o directorio
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Obtiene los atributos del archivo o directorio.

**Returns:**
int - los atributos del archivo o directorio
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Obtiene la ruta completa de la entrada dentro de la imagen.

**Returns:**
java.lang.String - la ruta completa de la entrada dentro de la imagen
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Obtiene el ID del enlace duro del archivo o directorio.

**Returns:**
long - el ID de enlace duro del archivo o directorio
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Obtiene la imagen a la que pertenece la entrada.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Obtiene la última hora de acceso del archivo o directorio.

**Returns:**
java.util.Date - la última hora de acceso del archivo o directorio
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Obtiene la hora de modificación del archivo o directorio.

**Returns:**
java.util.Date - la hora de modificación del archivo o directorio
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtiene la hora de modificación del archivo o directorio.

**Returns:**
java.util.Date - la hora de modificación del archivo o directorio
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada dentro de la imagen.

**Returns:**
java.lang.String - el nombre de la entrada dentro de la imagen
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Obtiene el directorio padre al que pertenece la entrada.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Obtiene el nombre corto de la entrada dentro de la imagen.

**Returns:**
java.lang.String - el nombre corto de la entrada dentro de la imagen
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Obtiene si el archivo o directorio es conocido por otros nombres.

**Returns:**
boolean - si el archivo o directorio es conocido por otros nombres
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtiene un valor que indica si la entrada representa un directorio.

**Returns:**
boolean - un valor que indica si la entrada representa un directorio
### toString() {#toString--}
```
public String toString()
```


Devuelve la representación en cadena de la instancia de la clase [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - representación en cadena de este objeto
