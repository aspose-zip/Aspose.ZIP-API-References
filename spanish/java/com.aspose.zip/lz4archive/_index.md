---
title: "Lz4Archive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo LZ4."
type: docs
weight: 80
url: /es/java/com.aspose.zip/lz4archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class Lz4Archive implements IArchive, IArchiveFileEntry, AutoCloseable
```

Esta clase representa un archivo LZ4. Úsela para extraer o componer archivos LZ4.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Lz4Archive(InputStream sourceStream)](#Lz4Archive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para descomprimir. |
| [Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)](#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-) | Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para descomprimir. |
| [Lz4Archive(String path)](#Lz4Archive-java.lang.String-) | Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive(String path, Lz4LoadOptions loadOptions)](#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-) | Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive). |
| [Lz4Archive()](#Lz4Archive--) | Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para comprimir. |
| [Lz4Archive(Lz4ArchiveSetting settings)](#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-) | Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para comprimir. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae el archivo al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae el archivo al archivo mediante la ruta. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae el contenido del archivo al directorio proporcionado. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [getLength()](#getLength--) | Obtiene la longitud. |
| [getName()](#getName--) | Obtiene el nombre original. |
| [open()](#open--) | Abre el archivo para extracción y proporciona un flujo con el contenido del archivo. |
| [save(File destination)](#save-java.io.File-) | Guarda el archivo lz4 en el archivo de destino proporcionado. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Guarda el archivo lz4 en el flujo proporcionado. |
| [save(String destinationFileName)](#save-java.lang.String-) | Guarda el archivo en el archivo de destino proporcionado. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(TarArchive tarArchive, TarFormat format)](#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(File fileInfo)](#setSource-java.io.File-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Establece el contenido que se comprimirá dentro del archivo. |
| [setSource(String path)](#setSource-java.lang.String-) | Establece el contenido que se comprimirá dentro del archivo. |
### Lz4Archive(InputStream sourceStream) {#Lz4Archive-java.io.InputStream-}
```
public Lz4Archive(InputStream sourceStream)
```


Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para descomprimir.

Abra un archivo desde un flujo y extráigalo a un `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(new FileInputStream(\"archive.lz4\"))) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions) {#Lz4Archive-java.io.InputStream-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(InputStream sourceStream, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive(new FileInputStream("archive.lz4"))) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Este constructor no descomprime. Vea el método [open()](../../com.aspose.zip/lz4archive\#open--) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Las opciones con las que cargar el archivo. |

### Lz4Archive(String path) {#Lz4Archive-java.lang.String-}
```
public Lz4Archive(String path)
```


Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive).

Abrir un archivo desde la ruta del archivo y extráigalo a un `MemoryStream`

```

``````

ByteArrayOutputStream ms = new ByteArrayOutputStream();
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
InputStream decompressed = archive.open();
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
ms.write(b, 0, bytesRead);
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/lz4archive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### Lz4Archive(String path, Lz4LoadOptions loadOptions) {#Lz4Archive-java.lang.String-com.aspose.zip.Lz4LoadOptions-}
```
public Lz4Archive(String path, Lz4LoadOptions loadOptions)
```


Initializes a new instance of the [Lz4Archive](../../com.aspose.zip/lz4archive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         InputStream decompressed = archive.open();
         byte[] b = new byte[8192];
         int bytesRead;
         while (0 < (bytesRead = decompressed.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
     }
 
```

Este constructor no descomprime. Vea el método [open()](../../com.aspose.zip/lz4archive\#open--) para descomprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |
| loadOptions | [Lz4LoadOptions](../../com.aspose.zip/lz4loadoptions) | Las opciones con las que cargar el archivo. |

### Lz4Archive() {#Lz4Archive--}
```
public Lz4Archive()
```


Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para comprimir.

### Lz4Archive(Lz4ArchiveSetting settings) {#Lz4Archive-com.aspose.zip.Lz4ArchiveSetting-}
```
public Lz4Archive(Lz4ArchiveSetting settings)
```


Inicializa una nueva instancia de la clase [Lz4Archive](../../com.aspose.zip/lz4archive) preparada para comprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| settings | [Lz4ArchiveSetting](../../com.aspose.zip/lz4archivesetting) | La configuración del archivo compuesto. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae el archivo al flujo proporcionado.

```

``````

OutputStream httpResponseStream = null;
try (Lz4Archive archive = new Lz4Archive(\"archive.lz4\")) {
archive.extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - info of an extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in. If the directory does not exist, it will be created |

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
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

``````

     try (Lz4Archive archive = new Lz4Archive("archive.lz4")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Lea del flujo para obtener el contenido original de un archivo. Vea la sección de ejemplos.

**Returns:**
java.io.InputStream - el flujo que representa el contenido del archivo
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Guarda el archivo lz4 en el archivo de destino proporcionado.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new File("data.bin"));
archive.save(new File(\"archive.lz4\"));
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | File, which will be opened as destination stream. |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lz4 archive to the stream provided.

```

``````

     try (FileOutputStream lz4File = new FileOutputStream("archive.lz4")) {
         try (Lz4Archive archive = new Lz4Archive()) {
             archive.setSource("data.bin");
             archive.save(lz4File);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| output | java.io.OutputStream | Flujo de destino. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Guarda el archivo en el archivo de destino proporcionado.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(\"data.bin\");
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

``````

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (Lz4Archive lz4Archive = new Lz4Archive()) {
             lz4Archive.setSource(tarArchive);
             lz4Archive.save("archive.tar.lz4");
         }
     }
 
```

Utilice este método para componer un archivo tar.lz4 conjunto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Archivo Tar que se comprimirá. |

### setSource(TarArchive tarArchive, TarFormat format) {#setSource-com.aspose.zip.TarArchive-com.aspose.zip.TarFormat-}
```
public final void setSource(TarArchive tarArchive, TarFormat format)
```


Establece el contenido que se comprimirá dentro del archivo.

```

``````

try (TarArchive tarArchive = new TarArchive()) {
tarArchive.createEntry("first.bin", "data1.bin");
tarArchive.createEntry("second.bin", "data2.bin");
try (Lz4Archive lz4Archive = new Lz4Archive()) {
lz4Archive.setSource(tarArchive);
lz4Archive.save("archive.tar.lz4");
}
}
 
```

Use this method to compose joint tar.lz4 archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |
| format | [TarFormat](../../com.aspose.zip/tarformat) | Defines tar header format. |

### setSource(File fileInfo) {#setSource-java.io.File-}
```
public final void setSource(File fileInfo)
```


Sets the content to be compressed within the archive.

Open an archive from a stream and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileInfo | java.io.File | La referencia a un archivo a comprimir. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Establece el contenido que se comprimirá dentro del archivo.

```

``````

try (Lz4Archive archive = new Lz4Archive()) {
archive.setSource(new ByteArrayInputStream(new byte[] {
0x00,
(byte) 0xFF
}));
archive.save(\"archive.lz4\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

``````

     try (Lz4Archive archive = new Lz4Archive()) {
         archive.setSource("data.bin");
         archive.save("archive.lz4");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | Ruta al archivo a comprimir. |

