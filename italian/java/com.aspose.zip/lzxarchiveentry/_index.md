---
title: "LzxArchiveEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno dell'archivio LZX."
type: docs
weight: 90
url: /it/java/com.aspose.zip/lzxarchiveentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class LzxArchiveEntry implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno dell'archivio LZX.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae l'entry dell'archivio Lzx in un filesystem tramite percorso. |
| [getCommentary()](#getCommentary--) | Ottiene il commento. |
| [getCompressedSize()](#getCompressedSize--) | Ottiene la dimensione del file compresso. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getModificationTime()](#getModificationTime--) | Ottiene l'ora dell'ultima modifica della voce. |
| [getName()](#getName--) | Restituisce il nome della voce. |
| [getUncompressedSize()](#getUncompressedSize--) | Ottiene la dimensione del file originale. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se questa voce è una directory. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | Flusso di destinazione. Deve essere scrivibile. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae l'entry dell'archivio Lzx in un filesystem tramite percorso.

```

``````

try (FileInputStream lzxFile = new FileInputStream(\"archive.lzx\")) {
try (LzxArchive archive = new LzxArchive(lzxFile)) {
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
### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Gets size of the compressed file.

**Returns:**
long - size of the compressed file.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Gets the last modified time of the entry.

**Returns:**
java.util.Date - the last modified time of the entry.
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry.

Archives for compression only, such as gzip, bzip2, lzip, lzma, xz, z has name "File.bin" unless another name can be found in headers.

**Returns:**
java.lang.String - the name of the entry
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of the original file.

**Returns:**
long - size of the original file.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether this entry is a directory.

**Returns:**
boolean - a value indicating whether this entry is a directory.
