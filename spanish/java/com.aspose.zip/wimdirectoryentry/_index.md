---
title: "WimDirectoryEntry"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Representa un solo directorio dentro del archivo wim."
type: docs
weight: 131
url: /es/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

Representa un solo directorio dentro del archivo wim.
## Métodos

| Método | Descripción |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrae todos los archivos del directorio actual al directorio proporcionado. |
| [getAllEntries()](#getAllEntries--) | Obtiene todas las entradas del tipo [WimEntry](../../com.aspose.zip/wimentry) que constituyen el directorio de forma recursiva. |
| [getDirectories()](#getDirectories--) | Obtiene entradas del tipo [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) que constituyen el directorio. |
| [getFiles()](#getFiles--) | Obtiene entradas del tipo [WimFileEntry](../../com.aspose.zip/wimfileentry) que constituyen el directorio. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Obtiene entradas del tipo [WimEntry](../../com.aspose.zip/wimentry) que constituyen el directorio. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrae todos los archivos del directorio actual al directorio proporcionado.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<WimEntry> getAllEntries()
```


Gets all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final List<WimDirectoryEntry> getDirectories()
```


Gets entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimDirectoryEntry&gt; - entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final List<WimFileEntry> getFiles()
```


Gets entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimFileEntry&gt; - entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<WimEntry> getFilesAndDirectories()
```


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory
