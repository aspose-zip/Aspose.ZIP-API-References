---
title: "AppleArchiveEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un file o una voce di directory all'interno di un ."
type: docs
weight: 17
url: /it/java/com.aspose.zip/applearchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public final class AppleArchiveEntry implements IArchiveFileEntry
```

Rappresenta un file o una voce di directory all'interno di un [AppleArchive](../../com.aspose.zip/applearchive).

Un'istanza di questa classe può rappresentare sia una voce analizzata da un Apple Archive esistente sia una voce aggiunta a un archivio in fase di composizione.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce dell'archivio Apple in un file system per percorso. |
| [getLength()](#getLength--) | Restituisce la lunghezza non compressa della voce in byte. |
| [getName()](#getName--) | Restituisce il percorso della voce all'interno dell'archivio. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [open()](#open--) | Apre la voce per l'estrazione e fornisce uno stream con il contenuto della voce. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | stream di destinazione. Deve essere scrivibile |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae la voce dell'archivio Apple in un file system per percorso.

```

``````

try (FileInputStream aaFile = new FileInputStream("archive.aa")) {
try (AppleArchive archive = new AppleArchive(aaFile)) {
archive.getEntries().get(0).extract("extracted.bin");
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file which will store decompressed data. |

**Returns:**
java.io.File - FileSystemInfoInstance containing extracted data.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the uncompressed length of the entry in bytes.

For directory entries the value is zero. For entries created from a non-seekable source stream the length can be unknown.

**Returns:**
java.lang.Long - the uncompressed length of the entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets the path of the entry inside the archive.

The value is the archive path recorded for the entry. Directory entries usually end with Forward slash (`/`).

**Returns:**
java.lang.String - the path of the entry inside the archive.
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


Opens the entry for extraction and provides a stream with the entry content.

**Returns:**
java.io.InputStream - A readable stream that contains the extracted entry data.
