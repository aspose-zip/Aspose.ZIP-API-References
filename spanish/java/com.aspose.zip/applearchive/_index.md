---
title: "AppleArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo Apple Archive .aar."
type: docs
weight: 16
url: /es/java/com.aspose.zip/applearchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AppleArchive implements IArchive, AutoCloseable
```

Esta clase representa un archivo Apple Archive (.aar). Úsela para crear archivos Apple Archive.

Apple y Apple Archive son marcas registradas de Apple Inc.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [AppleArchive()](#AppleArchive--) | Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) con la configuración utilizada para entradas compuestas. |
| [AppleArchive(AppleArchiveEntrySettings newEntrySettings)](#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-) | Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) con la configuración utilizada para entradas compuestas. |
| [AppleArchive(InputStream sourceStream)](#AppleArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo. |
| [AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-) | Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo. |
| [AppleArchive(String path)](#AppleArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo. |
| [AppleArchive(String path, AppleArchiveLoadOptions loadOptions)](#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-) | Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, File fileInfo, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crea una única entrada dentro del archivo. |
| [dispose()](#dispose--) | Ejecuta tareas definidas por la aplicación asociadas con la liberación, la liberación o el restablecimiento de recursos no administrados. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos del archivo al directorio proporcionado. |
| [getEntries()](#getEntries--) | Obtiene las entradas que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Obtiene la configuración utilizada para entradas recién compuestas. |
| [isSolid()](#isSolid--) | Obtiene un valor que indica si el archivo utiliza compresión sólida. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
### AppleArchive() {#AppleArchive--}
```
public AppleArchive()
```


Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) con la configuración utilizada para entradas compuestas.

### AppleArchive(AppleArchiveEntrySettings newEntrySettings) {#AppleArchive-com.aspose.zip.AppleArchiveEntrySettings-}
```
public AppleArchive(AppleArchiveEntrySettings newEntrySettings)
```


Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) con la configuración utilizada para entradas compuestas.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| newEntrySettings | [AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) | Configuración utilizada al crear un nuevo Apple Archive. |

### AppleArchive(InputStream sourceStream) {#AppleArchive-java.io.InputStream-}
```
public AppleArchive(InputStream sourceStream)
```


Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | sourceStream | java.io.InputStream | El origen del archivo. |

Este constructor no descomprime ninguna entrada. Consulte los métodos [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) y [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) para descomprimir. |

### AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.io.InputStream-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(InputStream sourceStream, AppleArchiveLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | El origen del archivo. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opciones para cargar el archivo existente. |

Este constructor no descomprime ninguna entrada. Consulte los métodos [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) y [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) para descomprimir. |

### AppleArchive(String path) {#AppleArchive-java.lang.String-}
```
public AppleArchive(String path)
```


Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | path | java.lang.String | La ruta completa o relativa al archivo. |

Este constructor no descomprime ninguna entrada. Consulte los métodos [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) y [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) para descomprimir. |

### AppleArchive(String path, AppleArchiveLoadOptions loadOptions) {#AppleArchive-java.lang.String-com.aspose.zip.AppleArchiveLoadOptions-}
```
public AppleArchive(String path, AppleArchiveLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [AppleArchive](../../com.aspose.zip/applearchive) y compone una lista de entradas que puede extraerse del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | La ruta completa o relativa al archivo. |
|  | loadOptions | [AppleArchiveLoadOptions](../../com.aspose.zip/applearchiveloadoptions) | Opciones para cargar el archivo existente. |

Este constructor no descomprime ninguna entrada. Consulte los métodos [extractToDirectory(String)](../../com.aspose.zip/applearchive\#extractToDirectory-String-) y [AppleArchiveEntry.open()](../../com.aspose.zip/applearchiveentry\#open--) para descomprimir. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final AppleArchive createEntries(File directory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.io.File | Directorio a comprimir. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final AppleArchive createEntries(File directory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.io.File | Directorio a comprimir. |
| includeRootDirectory | boolean | Indica si se debe incluir el directorio raíz o no. |

**Returns:**
[AppleArchive](../../com.aspose.zip/applearchive) - The archive with entries composed.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo)
```


Crea una única entrada dentro del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| fileInfo | java.io.File | Los metadatos del archivo a comprimir. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, File fileInfo, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final AppleArchiveEntry createEntry(String name, File fileInfo, boolean openImmediately)
```


Crea una única entrada dentro del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| fileInfo | java.io.File | Los metadatos del archivo a comprimir. |
| openImmediately | boolean | Verdadero, si se abre el archivo inmediatamente, de lo contrario se abre el archivo al guardar el archivo. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final AppleArchiveEntry createEntry(String name, InputStream source)
```


Crea una única entrada dentro del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| source | java.io.InputStream | El flujo de entrada para la entrada. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final AppleArchiveEntry createEntry(String name, String path)
```


Crea una única entrada dentro del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| path | java.lang.String | La ruta al archivo que se comprimirá. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final AppleArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Crea una única entrada dentro del archivo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| path | java.lang.String | La ruta al archivo que se comprimirá. |
| openImmediately | boolean | Verdadero, si se abre el archivo inmediatamente, de lo contrario se abre el archivo al guardar el archivo. |

**Returns:**
[AppleArchiveEntry](../../com.aspose.zip/applearchiveentry) - Apple Archive entry instance.
### dispose() {#dispose--}
```
public final void dispose()
```


Ejecuta tareas definidas por la aplicación asociadas con la liberación, la liberación o el restablecimiento de recursos no administrados.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrae todos los archivos del archivo al directorio proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | java.lang.String | La ruta al directorio donde colocar los archivos extraídos. |

### getEntries() {#getEntries--}
```
public final List<AppleArchiveEntry> getEntries()
```


Obtiene las entradas que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.AppleArchiveEntry&gt; - entradas que constituyen el archivo.
### getFileEntries() {#getFileEntries--}
```
public Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final AppleArchiveEntrySettings getNewEntrySettings()
```


Obtiene la configuración utilizada para entradas recién compuestas.

**Returns:**
[AppleArchiveEntrySettings](../../com.aspose.zip/applearchiveentrysettings) - settings used for newly composed entries.
### isSolid() {#isSolid--}
```
public final boolean isSolid()
```


Obtiene un valor que indica si el archivo utiliza compresión sólida. En modo sólido, todos los datos de las entradas se comprimen como una única secuencia y la extracción individual de entradas no está disponible. Use [IArchive.ExtractToDirectory()](../../com.aspose.zip/iarchive\#ExtractToDirectory--) en su lugar.

**Returns:**
boolean - un valor que indica si el archivo utiliza compresión sólida.
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Guarda el archivo en el flujo proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | output | java.io.OutputStream | Flujo de destino. |

`output` debe ser escribible. Algunas configuraciones de compresión, como LZ4, también requieren un flujo con capacidad de búsqueda. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Guarda el archivo en el archivo de destino proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | La ruta del archivo que se creará. |

