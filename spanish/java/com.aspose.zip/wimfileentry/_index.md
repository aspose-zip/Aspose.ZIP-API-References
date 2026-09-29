---
title: "WimFileEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo archivo dentro del archivo wim."
type: docs
weight: 133
url: /es/java/com.aspose.zip/wimfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class WimFileEntry extends WimEntry implements IArchiveFileEntry
```

Representa un solo archivo dentro del archivo wim.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

Extrae una entrada del archivo wim.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract(httpResponseStream);
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

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).getRootDirectory().getFiles().get(0).extract("data.bin");
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
### open() {#open--}
```
public final InputStream open()
```


Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada.

Uso:

```

``````

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
