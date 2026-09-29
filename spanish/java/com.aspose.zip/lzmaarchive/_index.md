---
title: "LzmaArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo LZMA."
type: docs
weight: 86
url: /es/java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Esta clase representa un archivo LZMA. Úsela para crear o extraer archivos LZMA.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) y compone el archivo en formato lzma. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) y compone el archivo en formato lzma. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparada para descomprimir. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparada para descomprimir. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extrae el archivo lzma a un archivo. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae el archivo lzma a un flujo. |
| [extract(String path)](#extract-java.lang.String-) | Extrae el archivo lzma a un archivo por ruta. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae el contenido del archivo al directorio proporcionado. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo lzma. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [getLength()](#getLength--) | Obtiene la longitud. |
| [getName()](#getName--) | El nombre del archivo original. |
| [save(File destination)](#save-java.io.File-) | Guarda el archivo lzma en el archivo de destino proporcionado. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo lzma en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo lzma en el archivo de destino proporcionado. |
| [setSource(File file)](#setSource-java.io.File-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Establece el contenido que se comprimirá dentro del archivo. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) y compone el archivo en formato lzma.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) y compone el archivo en formato lzma.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | conjunto de configuración del archivo lzma particular |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparada para descomprimir.

Este constructor no descomprime. Consulte el método [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Inicializa una nueva instancia de la clase [LzmaArchive](../../com.aspose.zip/lzmaarchive) preparada para descomprimir.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| file | java.io.File | el archivo para almacenar los datos descomprimidos |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae el archivo lzma a un flujo.

```

``````

try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
archive.extract(extractedFile);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

``````

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo que almacenará los datos descomprimidos |

**Returns:**
java.io.File - la información del archivo extraído
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrae el contenido del archivo al directorio proporcionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | destinationDirectory | java.lang.String | la ruta al directorio donde colocar los archivos extraídos. |

Si el directorio no existe, se creará |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo lzma.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo lzma.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtiene la longitud.

**Returns:**
java.lang.Long - longitud
### getName() {#getName--}
```
public final String getName()
```


El nombre del archivo original.

**Returns:**
java.lang.String - el nombre del archivo original
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Guarda el archivo lzma en el archivo de destino proporcionado.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.lzma"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

``````

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | flujo de destino |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Guarda el archivo lzma en el archivo de destino proporcionado.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| file | java.io.File | el archivo, que se abrirá como flujo de entrada |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Establece el contenido que se comprimirá dentro del archivo.

```

``````

try (LzmaArchive archive = new LzmaArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
archive.save("archive.lzma");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

``````

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourcePath | java.lang.String | ruta al archivo, que se abrirá como flujo de entrada |

