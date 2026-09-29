---
title: "SevenZipArchiveEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un archivo único dentro de un archivo 7z."
type: docs
weight: 105
url: /es/java/com.aspose.zip/sevenziparchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class SevenZipArchiveEntry implements IArchiveFileEntry
```

Representa un archivo único dentro de un archivo 7z.

Convierta una instancia de [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) a [SevenZipArchiveEntryEncrypted](../../com.aspose.zip/sevenziparchiveentryencrypted) para determinar si la entrada está encriptada o no.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getCompressedSize()](#getCompressedSize--) | Obtiene el tamaño del archivo comprimido. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [getCompressionSettings()](#getCompressionSettings--) | Obtiene la configuración para compresión o descompresión. |
| [getLength()](#getLength--) | Obtiene la longitud. |
| [getModificationTime()](#getModificationTime--) | Obtiene la fecha y hora de la última modificación. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño del archivo original. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada representa un directorio. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
| [open(String password)](#open-java.lang.String-) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

Extrae una entrada del archivo zip con contraseña.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Extracts the entry to the stream provided.

Extract an entry of zip archive with password.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destino | java.io.OutputStream | flujo de destino. Debe ser escribible |
| contraseña | java.lang.String | contraseña opcional para descifrado |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extrae la entrada al sistema de archivos mediante la ruta proporcionada.

```

``````

try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
archive.getEntries().get(0).extract("data.bin");
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

```

``````

     try (SevenZipArchive archive = new SevenZipArchive("archive.7z")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |
| contraseña | java.lang.String | contraseña opcional para descifrado |

**Returns:**
java.io.File - la información del archivo extraído
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Obtiene el tamaño del archivo comprimido.

**Returns:**
long - el tamaño del archivo comprimido
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

Event sender is an [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry) instance.

Does not invoke in solid mode and in multithreaded mode for LZMA2 entries.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getCompressionSettings() {#getCompressionSettings--}
```
public final SevenZipCompressionSettings getCompressionSettings()
```


Gets settings for compression or decompression.

**Returns:**
[SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings) - settings for compression or decompression
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


Gets the name of the entry within the archive.

**Returns:**
java.lang.String - the name of the entry within the archive
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets the size of the original file.

**Returns:**
long - the size of the original file
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents a directory.

**Returns:**
boolean - a value indicating whether the entry represents a directory
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

```

``````

     SevenZipArchive archive = new SevenZipArchive("archive.7z");
     SevenZipArchiveEntry entry = archive.getEntries().get(0);
     try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
         try (InputStream decompressed = entry.open()) {
             byte[] buffer = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
                 fileStream.write(buffer, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Lea del flujo para obtener el contenido original del archivo. Consulte la sección de ejemplos.

**Returns:**
java.io.InputStream - el flujo que representa el contenido de la entrada
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada.

Uso:

```

``````

SevenZipArchive archive = new SevenZipArchive("archive.7z");
SevenZipArchiveEntry entry = archive.getEntries().get(0);
try (FileOutputStream fileStream = new FileOutputStream("data.bin")) {
try (InputStream decompressed = entry.open()) {
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | optional password for decryption |

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
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

El remitente del evento es una instancia de [SevenZipArchiveEntry](../../com.aspose.zip/sevenziparchiveentry).

No se invoca en modo sólido y en modo multihilo para entradas LZMA2.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | un evento que se genera cuando una porción del flujo sin procesar se comprime. |

