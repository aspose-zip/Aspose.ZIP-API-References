---
title: "IsoEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un file o una directory di voce all'interno di un archivio ISO."
type: docs
weight: 72
url: /it/java/com.aspose.zip/isoentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class IsoEntry implements IArchiveFileEntry
```

Rappresenta una voce (file o directory) all'interno di un archivio ISO.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce nello stream fornito. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file system utilizzando il percorso fornito. |
| [getLength()](#getLength--) | Restituisce la lunghezza della voce. |
| [getModificationTime()](#getModificationTime--) | Restituisce la data e l'ora dell'ultima modifica. |
| [getName()](#getName--) | Restituisce il nome della voce. |
| [isDirectory()](#isDirectory--) | Restituisce un valore che indica se la voce è una directory. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta la voce corrente. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public void extract(OutputStream destination)
```


Estrae la voce nello stream fornito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | flusso di destinazione |

### extract(String path) {#extract-java.lang.String-}
```
public File extract(String path)
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
public Long getLength()
```


Restituisce la lunghezza della voce.

**Returns:**
java.lang.Long - la lunghezza della voce
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Restituisce la data e l'ora dell'ultima modifica.

**Returns:**
java.util.Date - data e ora dell'ultima modifica
### getName() {#getName--}
```
public final String getName()
```


Restituisce il nome della voce.

**Returns:**
java.lang.String - il nome della voce
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Restituisce un valore che indica se la voce è una directory.

**Returns:**
boolean - un valore che indica se la voce rappresenta una directory
### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta la voce corrente.

**Returns:**
java.lang.String - il nome della voce
