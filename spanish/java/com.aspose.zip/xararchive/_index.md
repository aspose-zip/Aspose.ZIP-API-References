---
title: "XarArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo xar."
type: docs
weight: 136
url: /es/java/com.aspose.zip/xararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XarArchive implements IArchive, AutoCloseable
```

Esta clase representa un archivo xar.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [XarArchive()](#XarArchive--) | Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(XarCompressionSettings defaultCompressionSettings)](#XarArchive-com.aspose.zip.XarCompressionSettings-) | Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive). |
| [XarArchive(InputStream sourceStream)](#XarArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive) y compone una lista de entradas que puede extraerse del archivo. |
| [XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)](#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-) | Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive) y compone una lista de entradas que puede extraerse del archivo. |
| [XarArchive(String path)](#XarArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive) y compone una lista de entradas que puede extraerse del archivo. |
| [XarArchive(String path, XarLoadOptions loadOptions)](#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-) | Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive) y compone una lista de entradas que puede extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)](#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-) | Crea una única entrada dentro del archivo. |
| [deleteEntry(XarEntry entry)](#deleteEntry-com.aspose.zip.XarEntry-) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos del archivo al directorio proporcionado. |
| [getEntries()](#getEntries--) | Obtiene entradas del tipo [XarEntry](../../com.aspose.zip/xarentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo xar. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo en el flujo proporcionado. |
| [save(OutputStream output, XarSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-) | Guarda el archivo en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
| [save(String destinationFileName, XarSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.XarSaveOptions-) | Guarda el archivo en el archivo de destino proporcionado. |
### XarArchive() {#XarArchive--}
```
public XarArchive()
```


Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive).

El siguiente ejemplo muestra cómo comprimir un archivo.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```



### XarArchive(XarCompressionSettings defaultCompressionSettings) {#XarArchive-com.aspose.zip.XarCompressionSettings-}
```
public XarArchive(XarCompressionSettings defaultCompressionSettings)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class.

The following example shows how to compress a file.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultCompressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | la configuración de compresión predeterminada, aplicada a todas las entradas del archivo. |

### XarArchive(InputStream sourceStream) {#XarArchive-java.io.InputStream-}
```
public XarArchive(InputStream sourceStream)
```


Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### XarArchive(InputStream sourceStream, XarLoadOptions loadOptions) {#XarArchive-java.io.InputStream-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(InputStream sourceStream, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive(new FileInputStream("archive.xar"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Este constructor no desempaqueta ninguna entrada. Consulte el método [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | las opciones para cargar el archivo. |

### XarArchive(String path) {#XarArchive-java.lang.String-}
```
public XarArchive(String path)
```


Inicializa una nueva instancia de la clase [XarArchive](../../com.aspose.zip/xararchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
archive.extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### XarArchive(String path, XarLoadOptions loadOptions) {#XarArchive-java.lang.String-com.aspose.zip.XarLoadOptions-}
```
public XarArchive(String path, XarLoadOptions loadOptions)
```


Initializes a new instance of the [XarArchive](../../com.aspose.zip/xararchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```

Este constructor no desempaqueta ninguna entrada. Consulte el método [XarFileEntry.open()](../../com.aspose.zip/xarfileentry\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |
| loadOptions | [XarLoadOptions](../../com.aspose.zip/xarloadoptions) | las opciones para cargar el archivo. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final XarArchive createEntries(File directory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.io.File | directorio a comprimir |
| includeRootDirectory | boolean | indica si se debe incluir el directorio raíz en sí o no |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(File directory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) items |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final XarArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directorio a comprimir |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
try (XarArchive archive = new XarArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(xarFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings) {#createEntries-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarArchive createEntries(String sourceDirectory, boolean includeRootDirectory, XarCompressionSettings compressionSettings)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream xarFile = new FileOutputStream("archive.xar")) {
         try (XarArchive archive = new XarArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(xarFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | java.lang.String | directorio a comprimir |
| includeRootDirectory | boolean | indica si se debe incluir el directorio raíz en sí o no |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | las configuraciones de compresión utilizadas para los elementos [XarEntry](../../com.aspose.zip/xarentry) añadidos |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final XarEntry createEntry(String name, File file)
```


Crea una única entrada dentro del archivo.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.xar");
     }
 
```

Si el archivo se abre inmediatamente con el parámetro `openImmediately`, queda bloqueado hasta que el archivo sea liberado

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| file | java.io.File | los metadatos del archivo o carpeta a comprimir |
| openImmediately | boolean | true si se abre el archivo inmediatamente, de lo contrario se abre al guardar el archivo |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, File file, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Crea una única entrada dentro del archivo.

```

``````

java.io.File file = new java.io.File("data.bin");
try (XarArchive archive = new XarArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.xar");
}
 
```

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving. |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final XarEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.xar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| source | java.io.InputStream | el flujo de entrada para la entrada |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, InputStream source, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, InputStream source, XarCompressionSettings compressionSettings)
```


Crea una única entrada dentro del archivo.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", new FileInputStream("data.bin"));
archive.save("archive.xar");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | the compression settings used for added [XarEntry](../../com.aspose.zip/xarentry) item |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final XarEntry createEntry(String name, String sourcePath)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `sourcePath` no afecta al nombre de la entrada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| sourcePath | java.lang.String | la ruta al archivo que se comprimirá |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Crea una única entrada dentro del archivo.

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.xar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |
| openImmediately | boolean | true, if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.XarCompressionSettings-}
```
public final XarEntry createEntry(String name, String sourcePath, boolean openImmediately, XarCompressionSettings compressionSettings)
```


Create a single entry within the archive.

```

``````

     try (XarArchive archive = new XarArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.xar");
     }
 
```

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `sourcePath` no afecta al nombre de la entrada.

Si el archivo se abre inmediatamente con el parámetro `openImmediately`, queda bloqueado hasta que el archivo se libere.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| sourcePath | java.lang.String | la ruta al archivo que se comprimirá |
| openImmediately | boolean | true, si se abre el archivo inmediatamente, de lo contrario abrir el archivo al guardar el archivo |
| compressionSettings | [XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings) | las configuraciones de compresión utilizadas para el elemento [XarEntry](../../com.aspose.zip/xarentry) añadido |

**Returns:**
[XarEntry](../../com.aspose.zip/xarentry) - Xar entry instance
### deleteEntry(XarEntry entry) {#deleteEntry-com.aspose.zip.XarEntry-}
```
public final XarArchive deleteEntry(XarEntry entry)
```


Elimina la primera aparición de una entrada específica de la lista de entradas.

Así es como puedes eliminar todas las entradas excepto la última:

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputXarFile.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | the entry to remove from the entries list |

**Returns:**
[XarArchive](../../com.aspose.zip/xararchive) - Xar entry instance
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (XarArchive archive = new XarArchive("archive.xar")) {
         archive.extractToDirectory("C:\\extracted");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | la ruta al directorio donde colocar los archivos extraídos. |

Si el directorio no existe, se creará |

### getEntries() {#getEntries--}
```
public final List<XarEntry> getEntries()
```


Obtiene entradas del tipo [XarEntry](../../com.aspose.zip/xarentry) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.XarEntry&gt; - entradas del tipo [XarEntry](../../com.aspose.zip/xarentry) que constituyen el archivo
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo xar.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo xar
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

Para archivos grandes, use [save(String)](../../com.aspose.zip/xararchive\#save-String-) en lugar de guardar en java.io.FileOutputStream.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | el flujo de destino |

### save(OutputStream output, XarSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.XarSaveOptions-}
```
public final void save(OutputStream output, XarSaveOptions saveOptions)
```


Guarda el archivo en el flujo proporcionado.

Para archivos grandes, use [save(String)](../../com.aspose.zip/xararchive\#save-String-) en lugar de guardar en java.io.FileOutputStream.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | el flujo de destino |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | las opciones para guardar el archivo xar con |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Guarda el archivo en el archivo de destino proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |

### save(String destinationFileName, XarSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.XarSaveOptions-}
```
public final void save(String destinationFileName, XarSaveOptions saveOptions)
```


Guarda el archivo en el archivo de destino proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |
| saveOptions | [XarSaveOptions](../../com.aspose.zip/xarsaveoptions) | las opciones para guardar el archivo xar con |

