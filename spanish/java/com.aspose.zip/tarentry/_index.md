---
title: "TarEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo dentro del archivo tar."
type: docs
weight: 126
url: /es/java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class TarEntry implements IArchiveFileEntry
```

Representa un solo archivo dentro del archivo tar.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getModificationTime()](#getModificationTime--) | Obtiene la hora de modificación del archivo o directorio. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [getUncompressedSize()](#getUncompressedSize--) | Obtiene el tamaño de un archivo original. |
| [isDirectory()](#isDirectory--) | Obtiene un valor que indica si la entrada representa un directorio. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
| [setName(String value)](#setName-java.lang.String-) | Establece el nombre de la entrada dentro del archivo. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

Extrae una entrada del archivo tar.

```

``````

try (TarArchive archive = new TarArchive(\"archive.tar\")) {
archive.getEntries().get_Item(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

**Returns:**
java.io.File - la información del archivo extraído
### getLength() {#getLength--}
```
public final Long getLength()
```


Obtiene la longitud de la entrada en bytes.

**Returns:**
java.lang.Long - la longitud de la entrada en bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Obtiene la hora de modificación del archivo o directorio.

**Returns:**
java.util.Date - la hora de modificación del archivo o directorio.
### getName() {#getName--}
```
public final String getName()
```


Obtiene el nombre de la entrada dentro del archivo.

**Returns:**
java.lang.String - el nombre de la entrada dentro del archivo
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Obtiene el tamaño de un archivo original.

Tiene el mismo valor que `Length`([getLength](../../com.aspose.zip/tarentry\#getLength--))

**Returns:**
long - el tamaño de un archivo original.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Obtiene un valor que indica si la entrada representa un directorio.

**Returns:**
boolean - un valor que indica si la entrada representa un directorio
### open() {#open--}
```
public final InputStream open()
```


Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada.


Uso:

```

``````

InputStream decompressed = entry.open();
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
fileStream.write(buffer, 0, bytesRead);
}
 
```

Read from the stream to get the original content of the file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets the name of the entry within the archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the name of the entry within the archive |

