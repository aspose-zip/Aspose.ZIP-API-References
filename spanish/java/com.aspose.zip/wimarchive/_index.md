---
title: "WimArchive"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Esta clase representa un archivo wim."
type: docs
weight: 130
url: /es/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Esta clase representa un archivo wim.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Inicializa una nueva instancia de la clase [WimArchive](../../com.aspose.zip/wimarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Inicializa una nueva instancia de la clase [WimArchive](../../com.aspose.zip/wimarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Inicializa una nueva instancia de la clase [WimArchive](../../com.aspose.zip/wimarchive) y compone una lista de entradas que puede extraerse del archivo. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Inicializa una nueva instancia de la clase [WimArchive](../../com.aspose.zip/wimarchive) y compone una lista de entradas que puede extraerse del archivo. |
## Métodos

| Método | Descripción |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae el archivo al archivo mediante la ruta. |
| [getBootImageIndex()](#getBootImageIndex--) | Obtiene el índice (basado en cero) de la imagen arrancable. |
| [getEntries()](#getEntries--) | Obtiene entradas del tipo [WimEntry](../../com.aspose.zip/wimentry) que constituyen el archivo. |
| [getFileEntries()](#getFileEntries--) | Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo wim. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Obtiene la versión del formato de archivo. |
| [getFormat()](#getFormat--) | Obtiene el formato del archivo. |
| [getGuid()](#getGuid--) | Obtiene el UUID identificador del archivo. |
| [getImages()](#getImages--) | Obtiene entradas del tipo [WimImage](../../com.aspose.zip/wimimage) que constituyen el archivo. |
| [getManifest()](#getManifest--) | Obtiene el manifiesto incrustado que describe el archivo y las imágenes contenidas. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Inicializa una nueva instancia de la clase [WimArchive](../../com.aspose.zip/wimarchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Este constructor no desempaqueta ninguna entrada. Consulte el método [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la fuente del archivo |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opciones para cargar el archivo existente. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Inicializa una nueva instancia de la clase [WimArchive](../../com.aspose.zip/wimarchive) y compone una lista de entradas que puede extraerse del archivo.

El siguiente ejemplo muestra cómo extraer todas las entradas a un directorio.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Este constructor no desempaqueta ninguna entrada. Consulte el método [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) para desempaquetar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| path | java.lang.String | la ruta al archivo del archivo |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opciones para cargar el archivo existente. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrae el archivo al archivo mediante la ruta.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| destinationDirectory | java.lang.String | la ruta al directorio donde colocar los archivos extraídos |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Obtiene el índice (basado en cero) de la imagen arrancable.

**Returns:**
int - el índice (basado en cero) de la imagen arrancable
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Obtiene entradas del tipo [WimEntry](../../com.aspose.zip/wimentry) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - entradas que constituyen el archivo
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Obtiene entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo wim.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entradas del tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) que constituyen el archivo wim
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Obtiene la versión del formato de archivo.

**Returns:**
int - la versión del formato de archivo
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Obtiene el formato del archivo.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Obtiene el UUID identificador del archivo.

**Returns:**
java.util.UUID - el UUID identificador del archivo
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Obtiene entradas del tipo [WimImage](../../com.aspose.zip/wimimage) que constituyen el archivo.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - entradas del tipo [WimImage](../../com.aspose.zip/wimimage) que constituyen el archivo
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Obtiene el manifiesto incrustado que describe el archivo y las imágenes contenidas.

**Returns:**
java.lang.String - el manifiesto incrustado que describe el archivo y las imágenes contenidas
