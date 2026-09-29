---
title: "CabArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo CAB."
type: docs
weight: 44
url: /es/java/com.aspose.zip/cabarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.zip.ICompressionArchive, java.lang.AutoCloseable
```
public class CabArchive implements ICompressionArchive, AutoCloseable
```

Esta clase representa un archivo CAB.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CabArchive(CabEntrySettings settings)](#CabArchive-com.aspose.zip.CabEntrySettings-) | Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) preparada para comprimir. |
| [CabArchive(InputStream sourceStream)](#CabArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)](#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-) | Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [CabArchive(String path)](#CabArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [CabArchive(String path, CabLoadOptions loadOptions)](#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-) | Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) y compone una lista de entradas que puede extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Agrega al archivo todos los archivos, recursivamente, del directorio especificado. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Agrega al archivo todos los archivos, recursivamente, del directorio especificado. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Agrega al archivo todos los archivos recursivamente desde la ruta del directorio especificado. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Agrega al archivo todos los archivos recursivamente desde la ruta del directorio especificado. |
| [createEntry(String name, File fileInfo)](#createEntry-java.lang.String-java.io.File-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-) | Crea una única entrada dentro del archivo con configuraciones específicas. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String path, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-) | Crea una única entrada dentro del archivo. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos del archivo al directorio proporcionado. |
| [getEntries()](#getEntries--) | Obtiene entradas del tipo [CabEntry](../../com.aspose.zip/cabentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo cab. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Guarda el archivo en el flujo proporcionado. |
| [save(OutputStream outputStream, CabSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-) | Guarda el archivo en el flujo proporcionado con opciones específicas. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
| [save(String destinationFileName, CabSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.CabSaveOptions-) | Guarda el archivo en el archivo de destino proporcionado. |
### CabArchive(CabEntrySettings settings) {#CabArchive-com.aspose.zip.CabEntrySettings-}
```
public CabArchive(CabEntrySettings settings)
```


Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) preparada para comprimir.

Comprime un archivo usando configuraciones de compresión específicas.

```

``````

CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings()));
try (CabArchive archive = new CabArchive(settings))
{
archive.createEntry(\"entry.bin\", \"data.bin\");
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | the source of the archive |

### CabArchive(InputStream sourceStream) {#CabArchive-java.io.InputStream-}
```
public CabArchive(InputStream sourceStream)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Este constructor no desempaqueta ninguna entrada. Consulte el método [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |

### CabArchive(InputStream sourceStream, CabLoadOptions loadOptions) {#CabArchive-java.io.InputStream-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(InputStream sourceStream, CabLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (CabArchive archive = new CabArchive(new FileInputStream("archive.cab"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### CabArchive(String path) {#CabArchive-java.lang.String-}
```
public CabArchive(String path)
```


Initializes a new instance of the [CabArchive](../../com.aspose.zip/cabarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Este constructor no desempaqueta ninguna entrada. Consulte el método [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

### CabArchive(String path, CabLoadOptions loadOptions) {#CabArchive-java.lang.String-com.aspose.zip.CabLoadOptions-}
```
public CabArchive(String path, CabLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [CabArchive](../../com.aspose.zip/cabarchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [CabEntry.open()](../../com.aspose.zip/cabentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| loadOptions | [CabLoadOptions](../../com.aspose.zip/cabloadoptions) | Options to load existing archive with. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final CabArchive createEntries(File directory)
```


Adds to the archive all files, recursively, from the specified directory.

```

``````

 try (var archive = new CabArchive())
 {
     File directory = new File("C:/Logs");
     archive.createEntries(directory);
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.io.File | Directorio a comprimir. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final CabArchive createEntries(File directory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos, recursivamente, del directorio especificado.

```

``````

try (var archive = new CabArchive())
{
File directory = new File("C:/Logs");
archive.createEntries(directory, false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final CabArchive createEntries(String sourceDirectory)
```


Adds to the archive all files recursively from the specified directory path.

```

``````

 try (var archive = new CabArchive())
 {
     archive.createEntries("C:/Logs");
     archive.save("logs.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Ruta del directorio a comprimir. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final CabArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos recursivamente desde la ruta del directorio especificado.

```

``````

try (var archive = new CabArchive())
{
archive.createEntries("C:/Logs", false);
archive.save("logs.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory path to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory name in entry paths. |

**Returns:**
[CabArchive](../../com.aspose.zip/cabarchive) - The current [CabArchive](../../com.aspose.zip/cabarchive) instance.
### createEntry(String name, File fileInfo) {#createEntry-java.lang.String-java.io.File-}
```
public final CabEntry createEntry(String name, File fileInfo)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     var sourceFile = new java.io.File("logs\\log.txt");
     archive.createEntry("log.txt", sourceFile);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
|  | fileInfo | java.io.File | Los metadatos del archivo a comprimir. |

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `fileInfo` no afecta al nombre de la entrada. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, File fileInfo, CabEntrySettings newEntrySettings)
```


Crea una única entrada dentro del archivo.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
File sourceFile = new File("logs\\log.txt");
archive.createEntry("log.txt", sourceFile, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| fileInfo | java.io.File | The metadata of file to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `fileInfo` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final CabEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
 {
     archive.createEntry("stream-entry.bin", stream);
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| source | java.io.InputStream | El flujo de entrada para la entrada. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, InputStream source, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, InputStream source, CabEntrySettings newEntrySettings)
```


Crea una única entrada dentro del archivo con configuraciones específicas.

```

``````

try (CabArchive archive = new CabArchive(); FileInputStream stream = new FileInputStream("stream-entry.bin"))
{
CabEntrySettings settings = new CabEntrySettings(new CabStoreCompressionSettings());
archive.createEntry("stream-entry.bin", stream, settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final CabEntry createEntry(String name, String path)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("entry.bin", "data.bin");
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
|  | path | java.lang.String | El nombre totalmente calificado del nuevo archivo, o el nombre de archivo relativo a comprimir. |

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `path` no afecta al nombre de la entrada. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, String path, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, String path, CabEntrySettings newEntrySettings)
```


Crea una única entrada dentro del archivo.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry("entry.bin", "data.bin", settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item.

The entry name is solely set within `name` parameter. The file name provided in `path` parameter does not affect the entry name. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - Cab entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider)
```


Create a single entry within the archive.

```

``````

 try (CabArchive archive = new CabArchive())
 {
     archive.createEntry("log.txt", () -> new FileInputStream("log.txt"));
     archive.save("archive.cab");
 } catch (IOException ex) {
 }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | El nombre de la entrada. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | El método que proporciona la secuencia de entrada para la entrada. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### createEntry(String name, Supplier&lt;InputStream&gt; streamProvider, CabEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.util.function.Supplier-java.io.InputStream--com.aspose.zip.CabEntrySettings-}
```
public final CabEntry createEntry(String name, Supplier<InputStream> streamProvider, CabEntrySettings newEntrySettings)
```


Crea una única entrada dentro del archivo.

```

``````

try (CabArchive archive = new CabArchive())
{
CabEntrySettings settings = new CabEntrySettings();
archive.createEntry("log.txt", () -> new FileInputStream("log.txt"), settings);
archive.save("archive.cab");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| streamProvider | java.util.function.Supplier&lt;java.io.InputStream&gt; | The method providing input stream for the entry. |
| newEntrySettings | [CabEntrySettings](../../com.aspose.zip/cabentrysettings) | Compression and encryption settings used for added [CabEntry](../../com.aspose.zip/cabentry) item. |

**Returns:**
[CabEntry](../../com.aspose.zip/cabentry) - CAB entry instance.
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | la ruta al directorio donde colocar los archivos extraídos. |

Si el directorio no existe, se creará |

### getEntries() {#getEntries--}
```
public final List<CabEntry> getEntries()
```


Obtiene entradas del tipo [CabEntry](../../com.aspose.zip/cabentry) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.CabEntry&gt; - entradas del tipo [CabEntry](../../com.aspose.zip/cabentry) que constituyen el archivo
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo cab.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo cab.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Guarda el archivo en el flujo proporcionado.

```

``````

try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
{
archive.createEntry(\"entry.bin\", \"data.bin\");
archive.save(cabFile);
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream.

`outputStream` must be writable. |

### save(OutputStream outputStream, CabSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.CabSaveOptions-}
```
public final void save(OutputStream outputStream, CabSaveOptions saveOptions)
```


Saves archive to the stream provided with specific options.

```

``````

  try (CabArchive archive = new CabArchive(); FileOutputStream cabFile = new FileOutputStream("archive.cab"))
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save(cabFile, options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Flujo de destino. |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | Opciones para guardar el archivo. |

`outputStream` debe ser escribible. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Guarda el archivo en el archivo de destino proporcionado.

```

``````

try (CabArchive archive = new CabArchive())
{
archive.createEntry(\"entry.bin\", \"data.bin\");
archive.save("archive.cab");
} catch (IOException ex) {
}
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to a temporary file. |

### save(String destinationFileName, CabSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.CabSaveOptions-}
```
public final void save(String destinationFileName, CabSaveOptions saveOptions)
```


Saves archive to the destination file provided.

```

``````

  try (CabArchive archive = new CabArchive())
  {
      CabSaveOptions options = new CabSaveOptions();
      options.setSkipChecksumCalculation(true);
      archive.createEntry("entry.bin", "data.bin");
      archive.save("archive.cab", options);
  } catch (IOException ex) {
  }
  
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | La ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |
|  | saveOptions | [CabSaveOptions](../../com.aspose.zip/cabsaveoptions) | Opciones para guardar el archivo. |

Es posible guardar un archivo en la misma ruta desde la que se cargó. Sin embargo, no se recomienda porque este enfoque utiliza la copia a un archivo temporal. |

