---
title: "LzxArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo de archivador LZX .lzx."
type: docs
weight: 89
url: /es/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Esta clase representa un archivo LZX (.lzx).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos y directorios del archivo al directorio proporcionado. |
| [getEntries()](#getEntries--) | Obtiene las entradas de archivo del tipo [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo.

Este constructor no descomprime ninguna entrada. Consulte el método [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extractionSource | java.io.InputStream | El origen del archivo. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo.

Este constructor no descomprime ninguna entrada. Consulte el método [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| extractionSource | java.io.InputStream | El origen del archivo. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opciones para cargar el archivo existente. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Inicializa una nueva instancia de la clase [LzxArchive](../../com.aspose.zip/lzxarchive) y compone una lista de entradas que pueden extraerse del archivo.

El siguiente ejemplo extrae un archivo, luego descomprime la primera entrada a un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive(\"sample.lzx\")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Este constructor no descomprime ninguna entrada. Consulte el método [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | La ruta completa o relativa al archivo. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opciones para cargar el archivo existente. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrae todos los archivos y directorios del archivo al directorio proporcionado.

```

``````

try (LzxArchive archive = new LzxArchive(\"archive.lzx\")) {
archive.extractToDirectory(\"C:/extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
