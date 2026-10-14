---
title: "LhaArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo LHA .lzh."
type: docs
weight: 75
url: /es/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Esta clase representa un archivo LHA (.lzh).

Solo se admiten los siguientes métodos de compresión:

| ------ | --------------------------------------------- |
| Método | Explicación                                   |
| lh0    | Sin comprimir                                  |
| lh4    | Diccionario deslizante de 8 KiB y Huffman estático   |
| lh5    | Diccionario deslizante de 16 KiB y Huffman estático  |
| lh6    | Diccionario deslizante de 64 KiB y Huffman estático  |
| lh7    | Diccionario deslizante de 128 KiB y Huffman estático |
| lhx    | Diccionario deslizante de 1 Mib y Huffman estático   |
| lhd    | Directorio                                     |
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos y directorios del archivo al directorio proporcionado. |
| [getEntries()](#getEntries--) | Obtiene las entradas de archivo del tipo [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo.

Este constructor no descomprime ninguna entrada. Consulte el método [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo.

Este constructor no descomprime ninguna entrada. Consulte el método [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opciones para cargar el archivo existente. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Inicializa una nueva instancia de la clase [LhaArchive](../../com.aspose.zip/lhaarchive) y compone una lista de entradas que pueden extraerse del archivo.

El siguiente ejemplo extrae un archivo, luego descomprime la primera entrada a un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Este constructor no descomprime ninguna entrada. Consulte el método [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta completa o la ruta relativa al archivo del archivo |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opciones para cargar el archivo existente. |

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

try (LhaArchive archive = new LhaArchive(\"archive.lzh\")) {
archive.extractToDirectory(\"C:/extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
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
