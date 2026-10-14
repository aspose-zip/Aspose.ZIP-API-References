---
title: "IArchiveFileEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa interfaccia rappresenta una voce di file di archivio."
type: docs
weight: 162
url: /it/java/com.aspose.zip/iarchivefileentry/
---
```
public interface IArchiveFileEntry
```

Questa interfaccia rappresenta una voce di file di archivio.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getLength()](#getLength--) | Ottiene la lunghezza della voce in byte. |
| [getName()](#getName--) | Restituisce il nome della voce. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public abstract void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | stream di destinazione. Deve essere scrivibile |

### extract(String path) {#extract-java.lang.String-}
```
public abstract File extract(String path)
```


Estrae la voce nel file system utilizzando il percorso fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di destinazione. Se il file esiste già, verrà sovrascritto |

**Returns:**
java.io.File - istanza java.io.File contenente i dati estratti
### getLength() {#getLength--}
```
public abstract Long getLength()
```


Ottiene la lunghezza della voce in byte.

**Returns:**
java.lang.Long - la lunghezza della voce in byte
### getName() {#getName--}
```
public abstract String getName()
```


Restituisce il nome della voce.

Gli archivi solo per compressione, come gzip, bzip2, lzip, lzma, xz, z, hanno il nome "File.bin" a meno che un altro nome possa essere trovato negli header.

**Returns:**
java.lang.String - il nome della voce
