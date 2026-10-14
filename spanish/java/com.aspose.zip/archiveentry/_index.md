---
title: "ArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un archivo único dentro del archivo."
type: docs
weight: 27
url: /es/java/com.aspose.zip/archiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class ArchiveEntry implements IArchiveFileEntry
```

Representa un archivo único dentro del archivo.

Convierta una instancia de [ArchiveEntry](../../com.aspose.zip/archiveentry) a [ArchiveEntryEncrypted](../../com.aspose.zip/archiveentryencrypted) para determinar si la entrada está encriptada o no.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getComment()](#getComment--) | Obtiene el comentario de la entrada dentro del archivo. |
| [getCompressedSize()](#getCompressedSize--) | Obtiene el tamaño del archivo comprimido. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtiene la configuración para compresión o descompresión. |
| [getDataSource()](#getDataSource--) | Origen de la entrada si la entrada fue añadida al archivo, no extraída. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Obtiene un evento que se dispara cuando se extrae una porción del flujo sin procesar. |
| [getLength()](#getLength--) | Obtiene la longitud. |
| [getModificationTime()](#getModificationTime--) | Obtiene la fecha y hora de la última modificación. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño del archivo original. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada representa un directorio. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |
| [open(String password)](#open-java.lang.String-) | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--) | Establece un evento que se dispara cuando se extrae una porción del flujo sin procesar. |
| [setModificationTime(Date value)](#setModificationTime-java.util.Date-) | Establece la fecha y hora de la última modificación. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

Extrae una entrada del archivo zip con contraseña.

```

``````

try (FileInputStream zipFile = new FileInputStream(\"archive.zip\")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(outputStream, \"p@s$\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract(outputStream, "p@s$");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | Flujo de destino. Debe ser escribible. |
| contraseña | java.lang.String | Contraseña opcional para descifrado. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

Extrae dos entradas del archivo ZIP, cada una con su propia contraseña

```

``````

try (FileInputStream zipFile = new FileInputStream(\"archive.zip\")) {
try (Archive archive = new Archive(zipFile)) {
archive.getEntries().get(0).extract(\"first.bin\", \"first_pass\");
archive.getEntries().get(1).extract(\"second.bin\", \"second_pass\");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of ZIP archive, each with own password

```

``````

    try (FileInputStream zipFile = new FileInputStream("archive.zip")) {
        try (Archive archive = new Archive(zipFile)) {
            archive.getEntries().get(0).extract("first.bin", "first_pass");
            archive.getEntries().get(1).extract("second.bin", "second_pass");
        }
    } catch (IOException ex) {
    }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | La ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |
| contraseña | java.lang.String | Contraseña opcional para descifrado. |

**Returns:**
java.io.File - la información del archivo extraído
### getComment() {#getComment--}
```
public final String getComment()
```


Obtiene el comentario de la entrada dentro del archivo.

**Returns:**
java.lang.String - comentario de la entrada dentro del archivo
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtiene el tamaño del archivo comprimido.

**Returns:**
long - tamaño del archivo comprimido
### getCompressionProgressed() {#getCompressionProgressed--}
```
public final Event<ProgressEventArgs> getCompressionProgressed()
```


Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final CompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[CompressionSettings](../../com.aspose.zip/compressionsettings) - settings for compression or decompression.
### getDataSource() {#getDataSource--}
```
public final InputStream getDataSource()
```


Source for the entry if the entry was added to the archive, not extracted.

Before assigned, the source is null. This source may be assigned within `Archive.save` method in some cases.

**Returns:**
java.io.InputStream - the source for the entry
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressCancelEventArgs> getExtractionProgressed()
```


Gets an event that is raised when a portion of raw stream extracted.

In this sample event handler is used for calculation the share of proceeded size in percents.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

En este ejemplo, el controlador de eventos se usa para la cancelación después de que se extrajeron los primeros cien Mb de la entrada.

```

``````

a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

Event sender is an [ArchiveEntry](../../com.aspose.zip/archiveentry) instance. It is possible to cancel extraction.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within the archive.

**Returns:**
java.lang.String - name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with decompressed entry content.


Usage:

```

``````

    InputStream decompressed = entry.open();
    byte[] buffer = new byte[8192];
    int bytesRead;
    while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
        fileStream.write(buffer, 0, bytesRead);
 
```

Lea del flujo para obtener el contenido original del archivo.

**Returns:**
java.io.InputStream - El flujo que representa el contenido de la entrada.
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada.


Uso:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length)))
fileStream.write(buffer, 0, bytesRead);
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | Optional password for decryption. |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream compressed.

```

``````

    archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
        }
    });
 
```

El remitente del evento es una instancia de [ArchiveEntry](../../com.aspose.zip/archiveentry).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento que se genera cuando una porción del flujo sin procesar se comprime. |

### setExtractionProgressed(Event&lt;ProgressCancelEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressCancelEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressCancelEventArgs> value)
```


Establece un evento que se dispara cuando se extrae una porción del flujo sin procesar.

En este ejemplo, el controlador de eventos se usa para calcular la proporción del tamaño procesado en porcentajes.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((ArchiveEntry) sender).getUncompressedSize());
}
});
 
```

In this sample event handler is used for cancellation after the first hundred of Mb of entry was extracted.

```

``````

 a.getEntries().get(0).setExtractionProgressed( (s, e) -> { if (e.getProceededBytes() > 100000000) e.setCancel(true); } );
 
```

El remitente del evento es una instancia de [ArchiveEntry](../../com.aspose.zip/archiveentry). Es posible cancelar la extracción.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.ProgressCancelEventArgs&gt; | un evento que se genera cuando se extrae una porción del flujo sin procesar. |

### setModificationTime(Date value) {#setModificationTime-java.util.Date-}
```
public final void setModificationTime(Date value)
```


Establece la fecha y hora de la última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | fecha y hora de última modificación |

