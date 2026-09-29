---
title: "WimDirectoryEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta una singola directory all'interno di un archivio wim."
type: docs
weight: 131
url: /it/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

Rappresenta una singola directory all'interno di un archivio wim.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file nella directory corrente nella directory fornita. |
| [getAllEntries()](#getAllEntries--) | Restituisce tutte le voci di tipo [WimEntry](../../com.aspose.zip/wimentry) che costituiscono la directory in modo ricorsivo. |
| [getDirectories()](#getDirectories--) | Restituisce le voci di tipo [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) che costituiscono la directory. |
| [getFiles()](#getFiles--) | Restituisce le voci di tipo [WimFileEntry](../../com.aspose.zip/wimfileentry) che costituiscono la directory. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Restituisce le voci di tipo [WimEntry](../../com.aspose.zip/wimentry) che costituiscono la directory. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae tutti i file nella directory corrente nella directory fornita.

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
