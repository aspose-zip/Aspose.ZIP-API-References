---
title: "ZArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo de compresión Z."
type: docs
weight: 153
url: /es/java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Esta clase representa un archivo Z (comprimido). Úsela para crear o extraer archivos Z.

Ver [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ZArchive()](#ZArchive--) | Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para comprimir. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extrae el archivo Z a un archivo. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae el archivo Z a un flujo. |
| [extract(String path)](#extract-java.lang.String-) | Extrae el archivo Z a un archivo mediante la ruta. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae el contenido del archivo al directorio proporcionado. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo Z. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo Z en el flujo proporcionado. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Guarda el archivo Z en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo Z en el archivo de destino proporcionado. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Guarda el archivo Z en el archivo de destino proporcionado. |
| [setSource(File file)](#setSource-java.io.File-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Establece el contenido que se comprimirá dentro del archivo. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para comprimir.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir.

Este constructor no descomprime. Consulte el método [extract(OutputStream)](../../com.aspose.zip/zarchive\\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir.

Este constructor no descomprime. Consulte el método [extract(OutputStream)](../../com.aspose.zip/zarchive\\#extract-OutputStream-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| source | java.io.InputStream | la fuente del archivo |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | las opciones para cargar el archivo. |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir.

Este constructor no descomprime. Consulte el método [extract(String)](../../com.aspose.zip/zarchive\\#extract-String-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al origen del archivo |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Inicializa una nueva instancia de la clase [ZArchive](../../com.aspose.zip/zarchive) preparada para descomprimir.

Este constructor no descomprime. Consulte el método [extract(String)](../../com.aspose.zip/zarchive\\#extract-String-) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al origen del archivo |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | las opciones para cargar el archivo. |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extrae el archivo Z a un archivo.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts Z archive to a stream.

```

``````

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | el flujo para almacenar datos descomprimidos |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae el archivo Z a un archivo mediante la ruta.

```

``````

try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
try (ZArchive archive = new ZArchive(zFile)) {
archive.extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

``````

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | el flujo de destino |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Guarda el archivo Z en el flujo proporcionado.

```

``````

try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
try (ZArchive archive = new ZArchive()) {
archive.setSource(\"data.bin\");
archive.save(zFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to the destination file provided.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Guarda el archivo Z en el archivo de destino proporcionado.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new File("data.bin"));
archive.save("data.bin.Z");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| file | java.io.File | la información del archivo que se abrirá como flujo de entrada |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Establece el contenido que se comprimirá dentro del archivo.

```

``````

try (ZArchive archive = new ZArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourcePath | java.lang.String | la ruta al archivo que se abrirá como flujo de entrada |

