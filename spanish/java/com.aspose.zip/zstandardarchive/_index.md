---
title: "ZstandardArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo Zstandard."
type: docs
weight: 156
url: /es/java/com.aspose.zip/zstandardarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZstandardArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

Esta clase representa un archivo Zstandard. Úsela para crear archivos Zstandard.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ZstandardArchive()](#ZstandardArchive--) | Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparada para comprimir. |
| [ZstandardArchive(InputStream sourceStream)](#ZstandardArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparada para descomprimir. |
| [ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)](#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-) | Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparada para descomprimir. |
| [ZstandardArchive(String path)](#ZstandardArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
| [ZstandardArchive(String path, ZstandardLoadOptions options)](#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-) | Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive). |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae el archivo al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae el archivo al archivo mediante la ruta. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae el contenido del archivo al directorio proporcionado. |
| [getFileEntries()](#getFileEntries--) | Obtiene las entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo zstandard. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [open()](#open--) | Abre el archivo para extracción y proporciona un flujo con el contenido del archivo. |
| [save(File destination)](#save-java.io.File-) | Guarda el archivo en el archivo de destino proporcionado. |
| [save(File destination, ZstandardSaveOptions settings)](#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-) | Guarda el archivo en el archivo de destino proporcionado. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Guarda el archivo en el flujo proporcionado. |
| [save(OutputStream outputStream, ZstandardSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-) | Guarda el archivo en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
| [save(String destinationFileName, ZstandardSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-) | Guarda el archivo en el archivo de destino proporcionado. |
| [setSource(File file)](#setSource-java.io.File-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(String path)](#setSource-java.lang.String-) | Establece el contenido que se comprimirá dentro del archivo. |
### ZstandardArchive() {#ZstandardArchive--}
```
public ZstandardArchive()
```


Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparada para comprimir.

El siguiente ejemplo muestra cómo comprimir un archivo.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(\"data.bin\");
archive.save("archive.zst");
}
 
```



### ZstandardArchive(InputStream sourceStream) {#ZstandardArchive-java.io.InputStream-}
```
public ZstandardArchive(InputStream sourceStream)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Este constructor no descomprime. Consulte el método [open()](../../com.aspose.zip/zstandardarchive\#open--) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |

### ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options) {#ZstandardArchive-java.io.InputStream-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(InputStream sourceStream, ZstandardLoadOptions options)
```


Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive) preparada para descomprimir.

Abrir un archivo desde un flujo y extraerlo a un `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive(new FileInputStream("archive.zst"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### ZstandardArchive(String path) {#ZstandardArchive-java.lang.String-}
```
public ZstandardArchive(String path)
```


Initializes a new instance of the [ZstandardArchive](../../com.aspose.zip/zstandardarchive) class.

Open an archive from file by path and extract it to a `ByteArrayOutputStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Este constructor no descomprime. Consulte el método [open()](../../com.aspose.zip/zstandardarchive\#open--) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |

### ZstandardArchive(String path, ZstandardLoadOptions options) {#ZstandardArchive-java.lang.String-com.aspose.zip.ZstandardLoadOptions-}
```
public ZstandardArchive(String path, ZstandardLoadOptions options)
```


Inicializa una nueva instancia de la clase [ZstandardArchive](../../com.aspose.zip/zstandardarchive).

Abrir un archivo desde una ruta y extraerlo a un `ByteArrayOutputStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/zstandardarchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |
| options | [ZstandardLoadOptions](../../com.aspose.zip/zstandardloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino. Debe ser escribible |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae el archivo al archivo mediante la ruta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

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


Obtiene las entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo zstandard.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo zstandard
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


Obtiene la longitud de la entrada en bytes.

**Returns:**
java.lang.Long - la longitud de la entrada en bytes
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada dentro del archivo.

**Returns:**
java.lang.String - el nombre de la entrada dentro del archivo
### open() {#open--}
```
public final InputStream open()
```


Abre el archivo para extracción y proporciona un flujo con el contenido del archivo.

Extrae el archivo y copia el contenido extraído al flujo de archivo.

```

``````

try (ZstandardArchive archive = new ZstandardArchive("archive.zst")) {
try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
InputStream unpacked = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
System.out.println(ex);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the archive
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.zst"));
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.File | el archivo que se abrirá como flujo de destino |

### save(File destination, ZstandardSaveOptions settings) {#save-java.io.File-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(File destination, ZstandardSaveOptions settings)
```


Guarda el archivo en el archivo de destino proporcionado.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(new File("archive.zst"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file, which will be opened as destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Write compressed data to http response stream.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(outputStream);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| outputStream | java.io.OutputStream | el flujo de destino |

### save(OutputStream outputStream, ZstandardSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(OutputStream outputStream, ZstandardSaveOptions settings)
```


Guarda el archivo en el flujo proporcionado.

Escribir datos comprimidos al flujo de respuesta http.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save(outputStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | the destination stream |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.zst");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationFileName | java.lang.String | la ruta del archivo que se creará. Si el nombre de archivo especificado apunta a un archivo existente, será sobrescrito |

### save(String destinationFileName, ZstandardSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZstandardSaveOptions-}
```
public final void save(String destinationFileName, ZstandardSaveOptions settings)
```


Guarda el archivo en el archivo de destino proporcionado.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new File("data.bin"));
archive.save("result.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZstandardSaveOptions](../../com.aspose.zip/zstandardsaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| file | java.io.File | la referencia a un archivo que será comprimido |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Establece el contenido que se comprimirá dentro del archivo.

```

``````

try (ZstandardArchive archive = new ZstandardArchive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save("archive.zst");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

```

``````

     try (ZstandardArchive archive = new ZstandardArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.zst");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | ruta al archivo a comprimir |

