---
title: "IArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta interfaz representa un archivo."
type: docs
weight: 161
url: /es/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Esta interfaz representa un archivo.
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos del archivo al directorio proporcionado. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Extrae todos los archivos del archivo al directorio proporcionado.

Si el directorio no existe, se creará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | java.lang.String | La ruta al directorio donde colocar los archivos extraídos. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo.

Los archivos para solo compresión, como gzip, bzip2, lzip, lzma, lz4, xz, z, consisten en un único registro: el propio archivo.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
