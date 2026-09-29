---
title: "CabEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo dentro del archivo cab."
type: docs
weight: 46
url: /es/java/com.aspose.zip/cabentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class CabEntry implements IArchiveFileEntry
```

Representa un solo archivo dentro del archivo cab.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [getModificationTime()](#getModificationTime--) | Obtiene la fecha y hora de la última modificación. |
| [getName()](#getName--) | Obtiene el nombre de la entrada dentro del archivo. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
| [toString()](#toString--) | Devuelve la representación en cadena de la instancia de la clase [CabEntry](../../com.aspose.zip/cabentry). |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

Extrae una entrada del archivo CAB.

```

``````

try (CabArchive archive = new CabArchive("archive.cab")) {
archive.getEntries().get(0).extract(httpResponseStream);
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream. Must be writable |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

```

``````

     try (CabArchive archive = new CabArchive("archive.cab")) {
         archive.getEntries().get(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

**Returns:**
java.io.File - la información del archivo de un archivo compuesto
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


Obtiene la fecha y hora de la última modificación.

**Returns:**
java.util.Date - fecha y hora de la última modificación.
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


Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada.

Uso:

```

``````

CabArchive archive = new CabArchive(\"archive.cab\");
CabEntry entry = archive.getEntries().get(0);
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

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - the stream that represents the contents of the entry
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the instance of the [CabEntry](../../com.aspose.zip/cabentry) class.

**Returns:**
java.lang.String - string representation of this object
