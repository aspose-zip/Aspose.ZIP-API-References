---
title: "IsoArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un archivo ISO ISO 9660."
type: docs
weight: 71
url: /es/java/com.aspose.zip/isoarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public final class IsoArchive implements IArchive, AutoCloseable
```

Representa un archivo ISO (ISO 9660).
## Constructores

| Constructor | Descripción |
| --- | --- |
| [IsoArchive()](#IsoArchive--) | Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y crea un archivo ISO vacío para agregar nuevos archivos y directorios. |
| [IsoArchive(InputStream sourceStream)](#IsoArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)](#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-) | Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [IsoArchive(String path)](#IsoArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [IsoArchive(String path, IsoLoadOptions loadOptions)](#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-) | Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y compone una lista de entradas que puede extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createDirectory(String name)](#createDirectory-java.lang.String-) | Agrega un directorio a la imagen ISO. |
| [createEntry(String name)](#createEntry-java.lang.String-) | Agrega un archivo a la imagen ISO. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Agrega un archivo a la imagen ISO. |
| [createEntry(String name, String filePath)](#createEntry-java.lang.String-java.lang.String-) | Agrega un archivo a la imagen ISO. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todas las entradas al directorio especificado. |
| [getEntries()](#getEntries--) | Obtiene entradas del tipo [IsoEntry](../../com.aspose.zip/isoentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Guarda la imagen ISO en el flujo especificado. |
| [save(OutputStream stream, IsoSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-) | Guarda la imagen ISO en el flujo especificado. |
| [save(String path)](#save-java.lang.String-) | Guarda la imagen ISO en la ruta especificada. |
| [save(String path, IsoSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.IsoSaveOptions-) | Guarda la imagen ISO en la ruta especificada. |
### IsoArchive() {#IsoArchive--}
```
public IsoArchive()
```


Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y crea un archivo ISO vacío para agregar nuevos archivos y directorios.

El siguiente ejemplo muestra cómo crear un nuevo archivo ISO vacío y agregar archivos a él:

```

``````

// Crear un nuevo archivo ISO vacío
try (IsoArchive isoArchive = new IsoArchive()) {
// Agregar archivos al archivo ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Guardar el archivo ISO en un archivo
isoArchive.save("new_archive.iso");
}
 
```



### IsoArchive(InputStream sourceStream) {#IsoArchive-java.io.InputStream-}
```
public IsoArchive(InputStream sourceStream)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Este constructor no desempaqueta ninguna entrada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |

### IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions) {#IsoArchive-java.io.InputStream-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(InputStream sourceStream, IsoLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### IsoArchive(String path) {#IsoArchive-java.lang.String-}
```
public IsoArchive(String path)
```


Initializes a new instance of the [IsoArchive](../../com.aspose.zip/isoarchive) class and composes an entry list that can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (IsoArchive archive = new IsoArchive("archive.iso")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Este constructor no desempaqueta ninguna entrada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

### IsoArchive(String path, IsoLoadOptions loadOptions) {#IsoArchive-java.lang.String-com.aspose.zip.IsoLoadOptions-}
```
public IsoArchive(String path, IsoLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [IsoArchive](../../com.aspose.zip/isoarchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (IsoArchive archive = new IsoArchive(\"archive.iso\")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [IsoLoadOptions](../../com.aspose.zip/isoloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### createDirectory(String name) {#createDirectory-java.lang.String-}
```
public final IsoEntry createDirectory(String name)
```


Adds a directory to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the directory in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name) {#createEntry-java.lang.String-}
```
public final IsoEntry createEntry(String name)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final IsoEntry createEntry(String name, InputStream source)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| source | java.io.InputStream | the stream containing the file data |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### createEntry(String name, String filePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final IsoEntry createEntry(String name, String filePath)
```


Adds a file to the ISO image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the path of the file in the ISO |
| filePath | java.lang.String | the path of the file |

**Returns:**
[IsoEntry](../../com.aspose.zip/isoentry) - the ISO entry composed
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

``````

     try (IsoArchive archive = new IsoArchive(new FileInputStream("archive.iso"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | java.lang.String | el directorio al que extraer las entradas |

### getEntries() {#getEntries--}
```
public final List<IsoEntry> getEntries()
```


Obtiene entradas del tipo [IsoEntry](../../com.aspose.zip/isoentry) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.IsoEntry&gt; - entradas del tipo [IsoEntry](../../com.aspose.zip/isoentry) que constituyen el archivo iso
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo iso
### getFormat() {#getFormat--}
```
public ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream stream)
```


Guarda la imagen ISO en el flujo especificado.

El siguiente ejemplo muestra cómo guardar un archivo ISO en un flujo de memoria:

```

``````

ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
// Crear un nuevo archivo ISO vacío
try (IsoArchive isoArchive = new IsoArchive()) {
// Agregar archivos al archivo ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Guardar el archivo ISO en un flujo de memoria
isoArchive.save(memoryStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the stream where the ISO image will be saved |

### save(OutputStream stream, IsoSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.IsoSaveOptions-}
```
public final void save(OutputStream stream, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified stream.

The following example shows how to save an ISO archive to a memory stream:

```

``````

     ByteArrayOutputStream memoryStream = new ByteArrayOutputStream();
     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a memory stream
         isoArchive.save(memoryStream);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| flujo | java.io.OutputStream | el flujo donde se guardará la imagen ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | las opciones para guardar el archivo ISO |

### save(String path) {#save-java.lang.String-}
```
public final void save(String path)
```


Guarda la imagen ISO en la ruta especificada.

El siguiente ejemplo muestra cómo guardar un archivo ISO en un archivo:

```

``````

// Crear un nuevo archivo ISO vacío
try (IsoArchive isoArchive = new IsoArchive()) {
// Agregar archivos al archivo ISO
isoArchive.createEntry("example_file.txt", "path_to_file.txt");
// Guardar el archivo ISO en un archivo
isoArchive.save("new_archive.iso");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path where the ISO image will be saved |

### save(String path, IsoSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.IsoSaveOptions-}
```
public final void save(String path, IsoSaveOptions saveOptions)
```


Saves the ISO image to the specified path.

The following example shows how to save an ISO archive to a file:

```

``````

     // Create a new empty ISO archive
     try (IsoArchive isoArchive = new IsoArchive()) {
         // Add files to the ISO archive
         isoArchive.createEntry("example_file.txt", "path_to_file.txt");
         // Save the ISO archive to a file
         isoArchive.save("new_archive.iso");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta donde se guardará la imagen ISO |
| saveOptions | [IsoSaveOptions](../../com.aspose.zip/isosaveoptions) | las opciones para guardar el archivo ISO |

