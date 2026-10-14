---
title: "RarArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un archivo único dentro del archivo."
type: docs
weight: 98
url: /es/java/com.aspose.zip/rararchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class RarArchiveEntry implements IArchiveFileEntry
```

Representa un archivo único dentro del archivo.

Convierta una instancia de [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) a [RarArchiveEntryEncrypted](../../com.aspose.zip/rararchiveentryencrypted) para determinar si la entrada está cifrada o no.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getCompressedSize()](#getCompressedSize--) | Obtiene el tamaño del archivo comprimido. |
| [getCreationTime()](#getCreationTime--) | Obtiene la fecha y hora de creación. |
| [getExtractionProgressed()](#getExtractionProgressed--) | Obtiene un evento que se dispara cuando se extrae una porción del flujo sin procesar. |
| [getLastAccessTime()](#getLastAccessTime--) | Obtiene la fecha y hora del último acceso. |
| [getLength()](#getLength--) | Obtiene la longitud. |
| [getModificationTime()](#getModificationTime--) | Obtiene la fecha y hora de la última modificación. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño del archivo original. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada representa un directorio. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |
| [open(String password)](#open-java.lang.String-) | Abre la entrada para extracción y proporciona un flujo con el contenido descomprimido de la entrada. |
| [setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Establece un evento que se dispara cuando se extrae una porción del flujo sin procesar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.


Extrae una entrada del archivo rar con contraseña.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
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


Extract an entry of rar archive with password.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
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


Extrae dos entradas del archivo rar.

```

``````

try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
try (RarArchive archive = new RarArchive(rarFile)) {
archive.getEntries().get(0).extract("first.bin", "pass");
archive.getEntries().get(1).extract("second.bin", "pass");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to destination file. If the file already exists, it will be overwritten |

**Returns:**
java.io.File - the file info of the extracted file
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Extracts the entry to the filesystem by the path provided.


Extract two entries of rar archive.

```

``````

    try (FileInputStream rarFile = new FileInputStream("archive.rar")) {
        try (RarArchive archive = new RarArchive(rarFile)) {
            archive.getEntries().get(0).extract("first.bin", "pass");
            archive.getEntries().get(1).extract("second.bin", "pass");
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
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtiene el tamaño del archivo comprimido.

**Returns:**
long - el tamaño del archivo comprimido
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Obtiene la fecha y hora de creación.

**Returns:**
java.util.Date - fecha y hora de creación.
### getExtractionProgressed() {#getExtractionProgressed--}
```
public final Event<ProgressEventArgs> getExtractionProgressed()
```


Obtiene un evento que se dispara cuando se extrae una porción del flujo sin procesar.

```

``````

archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
}
});
 
```

Event sender is an [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream extracted.
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Gets last access date and time.

**Returns:**
java.util.Date - last access date and time.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length.
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets last modified date and time.

**Returns:**
java.util.Date - last modified date and time.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file.
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

Lea del flujo para obtener el contenido original del archivo. Consulte la sección de ejemplos.

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
| password | java.lang.String | Optional password for decryption. It can also be set within [RarArchiveLoadOptions.setDecryptionPassword(String)](../../com.aspose.zip/rararchiveloadoptions\#setDecryptionPassword-String-). |

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setExtractionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setExtractionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setExtractionProgressed(Event<ProgressEventArgs> value)
```


Sets an event that is raised when a portion of raw stream extracted.

```

``````

    archive.getEntries().get(0).setExtractionProgressed(new Event<ProgressEventArgs>() {
        public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
            int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / ((RarArchiveEntry) sender).getUncompressedSize());
        }
    });
 
```

El remitente del evento es una instancia de [RarArchiveEntry](../../com.aspose.zip/rararchiveentry).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento que se genera cuando se extrae una porción del flujo sin procesar. |

