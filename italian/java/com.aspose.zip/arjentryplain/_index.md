---
title: "ArjEntryPlain"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file all'interno di un archivio ARJ."
type: docs
weight: 38
url: /it/java/com.aspose.zip/arjentryplain/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public class ArjEntryPlain implements IArchiveFileEntry
```

Rappresenta un singolo file all'interno di un archivio ARJ.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(File file)](#extract-java.io.File-) | Estrae una voce di archivio ARJ in un file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getCompressedSize()](#getCompressedSize--) | Restituisce la dimensione del file compresso. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Ottiene la dimensione del file originale. |
### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Estrae una voce di archivio ARJ in un file.

```

``````

try (FileInputStream arjFile = new FileInputStream("sourceFileName")) {
try (ArjArchive archive = new ArjArchive(arjFile)) {
archive.getEntries().get(0).extract(new File("extracted.bin"));
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | java.io.File for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the entry to the filesystem by the path provided.

Extract two entries of rar archive.

```

``````

     try (FileInputStream arjFile = new FileInputStream("archive.arj")) {
         try (ArjArchive archive = new ArjArchive(arjFile)) {
             archive.getEntries().get(0).extract("first.bin");
             archive.getEntries().get(1).extract("second.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |

**Returns:**
java.io.File - le informazioni sul file composto
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Restituisce la dimensione del file compresso.

**Returns:**
long - la dimensione del file compresso
### getLength() {#getLength--}
```
public final Long getLength()
```


Ottiene la lunghezza della voce in byte.

**Returns:**
java.lang.Long - la lunghezza della voce in byte
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome della voce all'interno dell'archivio.

**Returns:**
java.lang.String - nome della voce all'interno dell'archivio
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Ottiene la dimensione del file originale.

**Returns:**
long - dimensione del file originale
