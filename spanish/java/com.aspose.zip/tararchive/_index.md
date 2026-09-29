---
title: "TarArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo tar."
type: docs
weight: 125
url: /es/java/com.aspose.zip/tararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class TarArchive implements IArchive, AutoCloseable
```

Esta clase representa un archivo de archivador tar. Úsela para crear, extraer o actualizar archivos tar.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TarArchive()](#TarArchive--) | Inicializa una nueva instancia de la clase [TarArchive](../../com.aspose.zip/tararchive). |
| [TarArchive(InputStream sourceStream)](#TarArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [Archive](../../com.aspose.zip/archive) y compone una lista de entradas que puede extraerse del archivo. |
| [TarArchive(String path)](#TarArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [TarArchive](../../com.aspose.zip/tararchive) y compone una lista de entradas que se puede extraer del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source, File file)](#createEntry-java.lang.String-java.io.InputStream-java.io.File-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crea una única entrada dentro del archivo. |
| [deleteEntry(TarEntry entry)](#deleteEntry-com.aspose.zip.TarEntry-) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Elimina la entrada de la lista de entradas por índice. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos del archivo al directorio proporcionado. |
| [fromGZip(InputStream source)](#fromGZip-java.io.InputStream-) | Extrae el archivo gzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromGZip(String path)](#fromGZip-java.lang.String-) | Extrae el archivo gzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromLZ4(InputStream source)](#fromLZ4-java.io.InputStream-) | Extrae el archivo LZ4 suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromLZ4(String path)](#fromLZ4-java.lang.String-) | Extrae el archivo LZ4 suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromLZMA(InputStream source)](#fromLZMA-java.io.InputStream-) | Extrae el archivo LZMA suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromLZMA(String path)](#fromLZMA-java.lang.String-) | Extrae el archivo LZMA suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromLZip(InputStream source)](#fromLZip-java.io.InputStream-) | Extrae el archivo lzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromLZip(String path)](#fromLZip-java.lang.String-) | Extrae el archivo lzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromXz(InputStream source)](#fromXz-java.io.InputStream-) | Extrae el archivo en formato xz suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromXz(String path)](#fromXz-java.lang.String-) | Extrae el archivo en formato xz suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromZ(InputStream source)](#fromZ-java.io.InputStream-) | Extrae el archivo en formato Z suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromZ(String path)](#fromZ-java.lang.String-) | Extrae el archivo en formato Z suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromZstandard(InputStream source)](#fromZstandard-java.io.InputStream-) | Extrae el archivo Zstandard suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [fromZstandard(String path)](#fromZstandard-java.lang.String-) | Extrae el archivo Zstandard suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos. |
| [getEntries()](#getEntries--) | Obtiene las entradas del tipo [TarEntry](../../com.aspose.zip/tarentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene las entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo tar. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo en el flujo proporcionado. |
| [save(OutputStream output, TarFormat format)](#save-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
| [save(String destinationFileName, TarFormat format)](#save-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo de destino proporcionado. |
| [saveGzipped(OutputStream output)](#saveGzipped-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión gzip. |
| [saveGzipped(OutputStream output, TarFormat format)](#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión gzip. |
| [saveGzipped(String path)](#saveGzipped-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión gzip. |
| [saveGzipped(String path, TarFormat format)](#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión gzip. |
| [saveLZ4Compressed(OutputStream output)](#saveLZ4Compressed-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión LZ4. |
| [saveLZ4Compressed(OutputStream output, TarFormat format)](#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión LZ4. |
| [saveLZ4Compressed(String path)](#saveLZ4Compressed-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión LZ4. |
| [saveLZ4Compressed(String path, TarFormat format)](#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión LZ4. |
| [saveLZMACompressed(OutputStream output)](#saveLZMACompressed-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión LZMA. |
| [saveLZMACompressed(OutputStream output, TarFormat format)](#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión LZMA. |
| [saveLZMACompressed(String path)](#saveLZMACompressed-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión lzma. |
| [saveLZMACompressed(String path, TarFormat format)](#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión lzma. |
| [saveLzipped(OutputStream output)](#saveLzipped-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión lzip. |
| [saveLzipped(OutputStream output, TarFormat format)](#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión lzip. |
| [saveLzipped(String path)](#saveLzipped-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión lzip. |
| [saveLzipped(String path, TarFormat format)](#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión lzip. |
| [saveXzCompressed(OutputStream output)](#saveXzCompressed-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión xz. |
| [saveXzCompressed(OutputStream output, TarFormat format)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión xz. |
| [saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Guarda el archivo en el flujo con compresión xz. |
| [saveXzCompressed(String path)](#saveXzCompressed-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión xz. |
| [saveXzCompressed(String path, TarFormat format)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión xz. |
| [saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)](#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-) | Guarda el archivo en el archivo por ruta con compresión xz. |
| [saveZCompressed(OutputStream output)](#saveZCompressed-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión Z. |
| [saveZCompressed(OutputStream output, TarFormat format)](#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión Z. |
| [saveZCompressed(String path)](#saveZCompressed-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión Z. |
| [saveZCompressed(String path, TarFormat format)](#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión Z. |
| [saveZstandard(OutputStream output)](#saveZstandard-java.io.OutputStream-) | Guarda el archivo en el flujo con compresión Zstandard. |
| [saveZstandard(OutputStream output, TarFormat format)](#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-) | Guarda el archivo en el flujo con compresión Zstandard. |
| [saveZstandard(String path)](#saveZstandard-java.lang.String-) | Guarda el archivo en el archivo por ruta con compresión Zstandard. |
| [saveZstandard(String path, TarFormat format)](#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-) | Guarda el archivo en el archivo por ruta con compresión Zstandard. |
### TarArchive() {#TarArchive--}
```
public TarArchive()
```


Inicializa una nueva instancia de la clase [TarArchive](../../com.aspose.zip/tararchive).

El siguiente ejemplo muestra cómo comprimir un archivo.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(\"archive.tar\");
}
 
```



### TarArchive(InputStream sourceStream) {#TarArchive-java.io.InputStream-}
```
public TarArchive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (TarArchive archive = new TarArchive(new FileInputStream("archive.tar"))) {
             archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Este constructor no desempaqueta ninguna entrada. Vea el método [TarEntry.open()](../../com.aspose.zip/tarentry\\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |

### TarArchive(String path) {#TarArchive-java.lang.String-}
```
public TarArchive(String path)
```


Inicializa una nueva instancia de la clase [TarArchive](../../com.aspose.zip/tararchive) y compone una lista de entradas que se puede extraer del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [TarEntry.open()](../../com.aspose.zip/tarentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final TarArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.io.File | directorio a comprimir |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final TarArchive createEntries(File directory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final TarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directorio a comprimir |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final TarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with entries composed
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final TarEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     File fi = new File("data.bin");
     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("data.bin", fi);
         archive.save(tarFile);
     }
 
```

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `file` no afecta al nombre de la entrada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| file | java.io.File | los metadatos del archivo o carpeta a comprimir |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final TarEntry createEntry(String name, File file, boolean openImmediately)
```


Crea una única entrada dentro del archivo.

```

``````

File fi = new File(\"data.bin\");
try (TarArchive archive = new TarArchive()) {
archive.createEntry("data.bin", fi);
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final TarEntry createEntry(String name, InputStream source)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("bytes", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
         archive.save(tarFile);
     }
 
```

El nombre de la entrada se establece únicamente dentro del parámetro `name`.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| source | java.io.InputStream | el flujo de entrada para la entrada |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, InputStream source, File file) {#createEntry-java.lang.String-java.io.InputStream-java.io.File-}
```
public final TarEntry createEntry(String name, InputStream source, File file)
```


Crea una única entrada dentro del archivo.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"bytes\", new ByteArrayInputStream(new byte[] {0x00, (byte) 0xFF}));
archive.save(tarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `file` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final TarEntry createEntry(String name, String path)
```


Creates a single entry within the archive.

```

``````

     try (TarArchive archive = new TarArchive()) {
             archive.createEntry(first.bin, "data.bin");
             archive.save(outputTarFile);
     }
 
```

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `path` no afecta al nombre de la entrada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| path | java.lang.String | ruta al archivo a comprimir |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final TarEntry createEntry(String name, String path, boolean openImmediately)
```


Crea una única entrada dentro del archivo.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(first.bin, "data.bin");
archive.save(outputTarFile);
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| path | java.lang.String | path to file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[TarEntry](../../com.aspose.zip/tarentry) - Tar entry instance
### deleteEntry(TarEntry entry) {#deleteEntry-com.aspose.zip.TarEntry-}
```
public final TarArchive deleteEntry(TarEntry entry)
```


Removes the first occurrence of a specific entry from the entry list.

Here is how you can remove all entries except the last one:

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get_Item(0));
         archive.save(outputTarFile);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entry | [TarEntry](../../com.aspose.zip/tarentry) | la entrada a eliminar de la lista de entradas |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final TarArchive deleteEntry(int entryIndex)
```


Elimina la entrada de la lista de entradas por índice.

```

``````

try (TarArchive archive = new TarArchive(\"two_files.tar\")) {
archive.deleteEntry(0);
archive.save(\"single_file.tar\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - the archive with the entry deleted
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Si el directorio no existe, se creará.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | java.lang.String | la ruta al directorio donde colocar los archivos extraídos |

### fromGZip(InputStream source) {#fromGZip-java.io.InputStream-}
```
public static TarArchive fromGZip(InputStream source)
```


Extrae el archivo gzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo gzip se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El flujo de extracción GZip no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable bajo el capó.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromGZip(String path) {#fromGZip-java.lang.String-}
```
public static TarArchive fromGZip(String path)
```


Extrae el archivo gzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo gzip se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El flujo de extracción GZip no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable bajo el capó.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(InputStream source) {#fromLZ4-java.io.InputStream-}
```
public static TarArchive fromLZ4(InputStream source)
```


Extrae el archivo LZ4 suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo LZ4 se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | source | java.io.InputStream | El origen del archivo. |

El flujo de extracción LZ4 no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZ4(String path) {#fromLZ4-java.lang.String-}
```
public static TarArchive fromLZ4(String path)
```


Extrae el archivo LZ4 suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo LZ4 se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta al archivo del archivo. |

El flujo de extracción LZ4 no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - An instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(InputStream source) {#fromLZMA-java.io.InputStream-}
```
public static TarArchive fromLZMA(InputStream source)
```


Extrae el archivo LZMA suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo LZMA se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El flujo de extracción LZMA no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZMA(String path) {#fromLZMA-java.lang.String-}
```
public static TarArchive fromLZMA(String path)
```


Extrae el archivo LZMA suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo LZMA se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El flujo de extracción LZMA no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(InputStream source) {#fromLZip-java.io.InputStream-}
```
public static TarArchive fromLZip(InputStream source)
```


Extrae el archivo lzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo lzip se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El flujo de extracción lzip no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromLZip(String path) {#fromLZip-java.lang.String-}
```
public static TarArchive fromLZip(String path)
```


Extrae el archivo lzip suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo lzip se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El flujo de extracción lzip no es buscable por la naturaleza del algoritmo de compresión. El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo. |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(InputStream source) {#fromXz-java.io.InputStream-}
```
public static TarArchive fromXz(InputStream source)
```


Extrae el archivo en formato xz suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo xz se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromXz(String path) {#fromXz-java.lang.String-}
```
public static TarArchive fromXz(String path)
```


Extrae el archivo en formato xz suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo xz se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

El archivo Tar proporciona la capacidad de extraer un registro arbitrario, por lo que debe operar con un flujo buscable internamente.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(InputStream source) {#fromZ-java.io.InputStream-}
```
public static TarArchive fromZ(InputStream source)
```


Extrae el archivo en formato Z suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo Z se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZ(String path) {#fromZ-java.lang.String-}
```
public static TarArchive fromZ(String path)
```


Extrae el archivo en formato Z suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo Z se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(InputStream source) {#fromZstandard-java.io.InputStream-}
```
public static TarArchive fromZstandard(InputStream source)
```


Extrae el archivo Zstandard suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo Zstandard se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### fromZstandard(String path) {#fromZstandard-java.lang.String-}
```
public static TarArchive fromZstandard(String path)
```


Extrae el archivo Zstandard suministrado y crea un [TarArchive](../../com.aspose.zip/tararchive) a partir de los datos extraídos.

Importante: el archivo Zstandard se extrae completamente dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

**Returns:**
[TarArchive](../../com.aspose.zip/tararchive) - an instance of [TarArchive](../../com.aspose.zip/tararchive)
### getEntries() {#getEntries--}
```
public final List<TarEntry> getEntries()
```


Obtiene las entradas del tipo [TarEntry](../../com.aspose.zip/tarentry) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.TarEntry&gt; - entradas del tipo [TarEntry](../../com.aspose.zip/tarentry) que constituyen el archivo
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene las entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo tar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo tar
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Guarda el archivo en el flujo proporcionado.

```

``````

try (FileOutputStream tarFile = new FileOutputStream(\"archive.tar\")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save(tarFile);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### save(OutputStream output, TarFormat format) {#save-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void save(OutputStream output, TarFormat format)
```


Saves archive to the stream provided.

```

``````

     try (FileOutputStream tarFile = new FileOutputStream("archive.tar")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(tarFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | flujo de destino. |

`output` debe ser escribible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Guarda el archivo en el archivo de destino proporcionado.

```

``````

try (TarArchive archive = new TarArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save("myarchive.tar");
}
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, TarFormat format) {#save-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void save(String destinationFileName, TarFormat format)
```


Saves archive to the destination file provided.

```

``````

     try (TarArchive archive = new TarArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("myarchive.tar");
     }
 
```

Es posible guardar un archivo en la misma ruta desde la que se cargó. Sin embargo, no se recomienda porque este enfoque utiliza la copia a un archivo temporal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | la ruta del archivo a crear. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveGzipped(OutputStream output) {#saveGzipped-java.io.OutputStream-}
```
public final void saveGzipped(OutputStream output)
```


Guarda el archivo en el flujo con compresión gzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped(result);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveGzipped(OutputStream output, TarFormat format) {#saveGzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with gzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.gz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveGzipped(result);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | flujo de destino. |

`output` debe ser escribible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveGzipped(String path) {#saveGzipped-java.lang.String-}
```
public final void saveGzipped(String path)
```


Guarda el archivo en el archivo por ruta con compresión gzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveGzipped("result.tar.gz");
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveGzipped(String path, TarFormat format) {#saveGzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveGzipped(String path, TarFormat format)
```


Saves archive to the file by path with gzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveGzipped("result.tar.gz");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveLZ4Compressed(OutputStream output) {#saveLZ4Compressed-java.io.OutputStream-}
```
public final void saveLZ4Compressed(OutputStream output)
```


Guarda el archivo en el flujo con compresión LZ4.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | Destination stream. |

### saveLZ4Compressed(OutputStream output, TarFormat format) {#saveLZ4Compressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZ4 compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz4")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZ4Compressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | Flujo de destino. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible. |

### saveLZ4Compressed(String path) {#saveLZ4Compressed-java.lang.String-}
```
public final void saveLZ4Compressed(String path)
```


Guarda el archivo en el archivo por ruta con compresión LZ4.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZ4Compressed("result.tar.lz4");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### saveLZ4Compressed(String path, TarFormat format) {#saveLZ4Compressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZ4Compressed(String path, TarFormat format)
```


Saves archive to the file by path with LZ4 compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZ4Compressed("result.tar.lz4");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible. |

### saveLZMACompressed(OutputStream output) {#saveLZMACompressed-java.io.OutputStream-}
```
public final void saveLZMACompressed(OutputStream output)
```


Guarda el archivo en el flujo con compresión LZMA.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed(result);
}
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLZMACompressed(OutputStream output, TarFormat format) {#saveLZMACompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with LZMA compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lzma")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLZMACompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```

Importante: el archivo tar se compone y luego se comprime dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | flujo de destino. |

`output` debe ser escribible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveLZMACompressed(String path) {#saveLZMACompressed-java.lang.String-}
```
public final void saveLZMACompressed(String path)
```


Guarda el archivo en el archivo por ruta con compresión lzma.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLZMACompressed("result.tar.lzma");
}
} catch (IOException ex) {
}
 
```

Important: tar archive is composed then compressed within this method, its content is kept internally. Beware of memory consumption.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLZMACompressed(String path, TarFormat format) {#saveLZMACompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLZMACompressed(String path, TarFormat format)
```


Saves archive to the file by path with lzma compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLZMACompressed("result.tar.lzma");
         }
     } catch (IOException ex) {
     }
 
```

Importante: el archivo tar se compone y luego se comprime dentro de este método, su contenido se mantiene internamente. Tenga en cuenta el consumo de memoria.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveLzipped(OutputStream output) {#saveLzipped-java.io.OutputStream-}
```
public final void saveLzipped(OutputStream output)
```


Guarda el archivo en el flujo con compresión lzip.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveLzipped(OutputStream output, TarFormat format) {#saveLzipped-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(OutputStream output, TarFormat format)
```


Saves archive to the stream with lzip compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.lz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveLzipped(result, TarFormat.Gnu);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | flujo de destino. |

`output` debe ser escribible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveLzipped(String path) {#saveLzipped-java.lang.String-}
```
public final void saveLzipped(String path)
```


Guarda el archivo en el archivo por ruta con compresión lzip.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveLzipped("result.tar.lz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveLzipped(String path, TarFormat format) {#saveLzipped-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveLzipped(String path, TarFormat format)
```


Saves archive to the file by path with lzip compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveLzipped("result.tar.lz", TarFormat.Gnu);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveXzCompressed(OutputStream output) {#saveXzCompressed-java.io.OutputStream-}
```
public final void saveXzCompressed(OutputStream output)
```


Guarda el archivo en el flujo con compresión xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |

### saveXzCompressed(OutputStream output, TarFormat format) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with xz compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveXzCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | flujo de destino. |

`output`El flujo debe ser escribible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(OutputStream output, TarFormat format, XzArchiveSettings settings)
```


Guarda el archivo en el flujo con compresión xz.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.xz")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output`The stream must be writable |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines the tar header format. Null value will be treated as USTar when possible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### saveXzCompressed(String path) {#saveXzCompressed-java.lang.String-}
```
public final void saveXzCompressed(String path)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |

### saveXzCompressed(String path, TarFormat format) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveXzCompressed(String path, TarFormat format)
```


Guarda el archivo en el archivo por ruta con compresión xz.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveXzCompressed("result.tar.xz");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| format | [TarFormat](../../com.aspose.zip/tarformat) | defines tar header format. Null value will be treated as USTar when possible |

### saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings) {#saveXzCompressed-java.lang.String-com.aspose.zip.TarFormat-com.aspose.zip.XzArchiveSettings-}
```
public final void saveXzCompressed(String path, TarFormat format, XzArchiveSettings settings)
```


Saves archive to the file by path with xz compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveXzCompressed("result.tar.xz");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | conjunto de configuraciones específicas del archivo xz: tamaño del diccionario, tamaño de bloque, tipo de verificación |

### saveZCompressed(OutputStream output) {#saveZCompressed-java.io.OutputStream-}
```
public final void saveZCompressed(OutputStream output)
```


Guarda el archivo en el flujo con compresión Z.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### saveZCompressed(OutputStream output, TarFormat format) {#saveZCompressed-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(OutputStream output, TarFormat format)
```


Saves archive to the stream with Z compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.Z")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZCompressed(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | el flujo de destino |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveZCompressed(String path) {#saveZCompressed-java.lang.String-}
```
public final void saveZCompressed(String path)
```


Guarda el archivo en el archivo por ruta con compresión Z.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZCompressed("result.tar.Z");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZCompressed(String path, TarFormat format) {#saveZCompressed-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZCompressed(String path, TarFormat format)
```


Saves archive to the file by path with Z compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZCompressed("result.tar.Z");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveZstandard(OutputStream output) {#saveZstandard-java.io.OutputStream-}
```
public final void saveZstandard(OutputStream output)
```


Guarda el archivo en el flujo con compresión Zstandard.

```

``````

try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard(result);
}
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream.

`output` must be writable |

### saveZstandard(OutputStream output, TarFormat format) {#saveZstandard-java.io.OutputStream-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(OutputStream output, TarFormat format)
```


Saves archive to the stream with Zstandard compression.

```

``````

     try (FileOutputStream result = new FileOutputStream("result.tar.zst")) {
         try (FileInputStream source = new FileInputStream("data.bin")) {
             try (TarArchive archive = new TarArchive()) {
                 archive.createEntry("entry.bin", source);
                 archive.saveZstandard(result);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | flujo de destino. |

`output` debe ser escribible |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

### saveZstandard(String path) {#saveZstandard-java.lang.String-}
```
public final void saveZstandard(String path)
```


Guarda el archivo en el archivo por ruta con compresión Zstandard.

```

``````

try (FileInputStream source = new FileInputStream("data.bin")) {
try (TarArchive archive = new TarArchive()) {
archive.createEntry("entry.bin", source);
archive.saveZstandard("result.tar.zst");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### saveZstandard(String path, TarFormat format) {#saveZstandard-java.lang.String-com.aspose.zip.TarFormat-}
```
public final void saveZstandard(String path, TarFormat format)
```


Saves archive to the file by path with Zstandard compression.

```

``````

     try (FileInputStream source = new FileInputStream("data.bin")) {
         try (TarArchive archive = new TarArchive()) {
             archive.createEntry("entry.bin", source);
             archive.saveZstandard("result.tar.zst");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| format | [TarFormat](../../com.aspose.zip/tarformat) | define el formato de cabecera tar. El valor nulo se tratará como USTar cuando sea posible |

