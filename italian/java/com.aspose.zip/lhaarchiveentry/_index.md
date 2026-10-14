---
title: "LhaArchiveEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno dell'archivio Lha."
type: docs
weight: 76
url: /it/java/com.aspose.zip/lhaarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LhaArchiveEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno dell'archivio Lha.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Estrae la voce dell'archivio Lha in un file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce dell'archivio Lha in un file system per percorso. |
| [getLastModified()](#getLastModified--) | Ottiene l'ora dell'ultima modifica della voce. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getModificationTime()](#getModificationTime--) | Ottiene l'ora dell'ultima modifica della voce. |
| [getName()](#getName--) | Restituisce il nome della voce. |
| [getPath()](#getPath--) | Ottiene il percorso completo della voce. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se questa voce è una directory. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Estrae la voce dell'archivio Lha in un file.

```

``````

try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
try (LhaArchive archive = new LhaArchive(lhaFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | File for storing decompressed data.

Does nothing for directory entry |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | destination stream |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts Lha archive entry to a filesystem by path.

```

``````

     try (FileInputStream lhaFile = new FileInputStream("archive.lha")) {
         try (LhaArchive archive = new LhaArchive(lhaFile)) {
             archive.getEntries().get(0).extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file che conterrà i dati decompressi |

**Returns:**
java.io.File - istanza java.io.File contenente i dati estratti
### getLastModified() {#getLastModified--}
```
public final Date getLastModified()
```


Ottiene l'ora dell'ultima modifica della voce.

**Returns:**
java.util.Date - l'ora dell'ultima modifica della voce
### getLength() {#getLength--}
```
public final Long getLength()
```


Ottiene la lunghezza della voce in byte.

**Returns:**
java.lang.Long - la lunghezza della voce in byte
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Ottiene l'ora dell'ultima modifica della voce.

**Returns:**
java.util.Date - l'ora dell'ultima modifica della voce
### getName() {#getName--}
```
public final String getName()
```


Restituisce il nome della voce.

Gli archivi solo per compressione, come gzip, bzip2, lzip, lzma, xz, z, hanno il nome "File.bin" a meno che un altro nome possa essere trovato negli header.

**Returns:**
java.lang.String - il nome della voce
### getPath() {#getPath--}
```
public final String getPath()
```


Ottiene il percorso completo della voce.

**Returns:**
java.lang.String - il percorso completo della voce
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ottiene un valore che indica se questa voce è una directory.

**Returns:**
boolean - un valore che indica se questa voce è una directory.
