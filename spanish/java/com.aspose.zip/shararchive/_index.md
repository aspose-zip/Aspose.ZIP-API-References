---
title: "SharArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo shar."
type: docs
weight: 119
url: /es/java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

Esta clase representa un archivo shar.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [SharArchive()](#SharArchive--) | Inicializa una nueva instancia de la clase [SharArchive](../../com.aspose.zip/shararchive). |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [SharArchive](../../com.aspose.zip/shararchive) preparada para descomprimir. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Crea una única entrada dentro del archivo. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Crea una única entrada dentro del archivo. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | Elimina la primera aparición de una entrada específica de la lista de entradas. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Elimina la entrada de la lista de entradas por índice. |
| [getEntries()](#getEntries--) | Obtiene entradas del tipo [SharEntry](../../com.aspose.zip/sharentry) que constituyen el archivo. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


Inicializa una nueva instancia de la clase [SharArchive](../../com.aspose.zip/shararchive).

El siguiente ejemplo muestra cómo comprimir un archivo.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| directorio | java.io.File | el directorio a comprimir |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries(new java.io.File("C:\\folder"), false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

``````

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceDirectory | java.lang.String | el directorio a comprimir |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Agrega al archivo todos los archivos y directorios de forma recursiva en el directorio especificado.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntries("C:\\folder", false);
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Creates a single entry within the archive.

```

``````

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| file | java.io.File | los metadatos del archivo o carpeta a comprimir |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


Crea una única entrada dentro del archivo.

```

``````

java.io.File file = new java.io.File("data.bin");
try (SharArchive archive = new SharArchive()) {
archive.createEntry(\"test.bin\", file);
archive.save("archive.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| source | java.io.InputStream | el flujo de entrada para la entrada |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


Crea una única entrada dentro del archivo.

```

``````

try (SharArchive archive = new SharArchive()) {
archive.createEntry("first.bin", "data.bin");
archive.save("archive.shar");
}
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create a single entry within the archive.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

El nombre de la entrada se establece únicamente dentro del parámetro `name`. El nombre de archivo proporcionado en el parámetro `sourcePath` no afecta al nombre de la entrada.

Si el archivo se abre inmediatamente con el parámetro `openImmediately`, queda bloqueado hasta que el archivo se libere.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String | el nombre de la entrada |
| sourcePath | java.lang.String | la ruta al archivo a comprimir |
| openImmediately | boolean | true, si se abre el archivo inmediatamente, de lo contrario abrir el archivo al guardar el archivo |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


Elimina la primera aparición de una entrada específica de la lista de entradas.

Así es como puedes eliminar todas las entradas excepto la última:

```

``````

try (SharArchive archive = new SharArchive("archive.shar")) {
while (archive.getEntries().size() > 1)
archive.deleteEntry(archive.getEntries().get(0));
archive.save("outputSharFile.shar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entry list by index.

```

``````

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| entryIndex | int | el índice basado en cero de la entrada a eliminar |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


Obtiene entradas del tipo [SharEntry](../../com.aspose.zip/sharentry) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - entradas de tipo [SharEntry](../../com.aspose.zip/sharentry) que constituyen el archivo
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Guarda el archivo en el flujo proporcionado.

```

``````

try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
try (SharArchive archive = new SharArchive()) {
archive.createEntry(\"entry1\", \"data.bin\");
archive.save(sharFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | destinationFileName | java.lang.String | la ruta del archivo a crear. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito. |

Es posible guardar un archivo en la misma ruta desde la que se cargó. Sin embargo, no se recomienda porque este enfoque utiliza la copia a un archivo temporal |

