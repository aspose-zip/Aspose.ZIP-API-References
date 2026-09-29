---
title: "XarFileEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa una entrada de archivo dentro del archivo xar."
type: docs
weight: 141
url: /es/java/com.aspose.zip/xarfileentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class XarFileEntry extends XarEntry implements IArchiveFileEntry
```

Representa una entrada de archivo dentro del archivo xar.
## Métodos

| Método | Descripción |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extrae la entrada al flujo proporcionado. |
| [extract(String path)](#extract-java.lang.String-) | Extrae la entrada al sistema de archivos mediante la ruta proporcionada. |
| [getCompressionProgressed()](#getCompressionProgressed--) | Obtiene un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
| [getLength()](#getLength--) | Obtiene la longitud de la entrada en bytes. |
| [open()](#open--) | Abre la entrada para extracción y proporciona un flujo con el contenido de la entrada. |
| [setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value)](#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--) | Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extrae la entrada al flujo proporcionado.

Extrae una entrada del archivo wim.

```

``````

try (FileOutputStream output = new FileOutputStream("file")){
try (XarArchive archive = new XarArchive("archive.xar")) {
((XarFileEntry)archive.getEntries().get(0)).extract(output);
}
} catch (IOException ex) {
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

     try (XarArchive archive = new XarArchive("archive.xar")) {
         ((XarFileEntry)archive.getEntries().get(0)).extract("data.bin");
     }
 
```



**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo de destino. Si el archivo ya existe, será sobrescrito. |

**Returns:**
java.io.File - la información del archivo extraído
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

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised when a portion of raw stream compressed
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.

Usage:

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

Lea del flujo para obtener el contenido original del archivo. Consulte la sección de ejemplos.

**Returns:**
java.io.InputStream - el flujo que representa el contenido de la entrada
### setCompressionProgressed(Event&lt;ProgressEventArgs&gt; value) {#setCompressionProgressed-com.aspose.zip.Event-com.aspose.zip.ProgressEventArgs--}
```
public final void setCompressionProgressed(Event<ProgressEventArgs> value)
```


Establece un evento que se dispara cuando se comprime una parte del flujo sin procesar.

```

``````

archive.getEntries().get(0).setCompressionProgressed(new Event<ProgressEventArgs>() {
public void invoke(Object sender, ProgressEventArgs progressEventArgs) {
int percent = (int) ((100 * (long) progressEventArgs.getProceededBytes()) / entrySourceFile.length());
}
});
 
```

Event sender is an [XarFileEntry](../../com.aspose.zip/xarfileentry) instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | com.aspose.zip.Event&lt;com.aspose.zip.ProgressEventArgs&gt; | an event that is raised when a portion of raw stream compressed |

