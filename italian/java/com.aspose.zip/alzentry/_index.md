---
title: "AlzEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta una voce di file in un archivio ALZ insieme ai relativi metadati."
type: docs
weight: 13
url: /it/java/com.aspose.zip/alzentry/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry)
```
public abstract class AlzEntry implements IArchiveFileEntry
```

Rappresenta una voce di file in un archivio ALZ insieme ai relativi metadati.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Estrae la voce in un flusso scrivibile. |
| [extract(OutputStream destination, String password)](#extract-java.io.OutputStream-java.lang.String-) | Estrae la voce in un flusso scrivibile usando una password opzionale. |
| [extract(String path)](#extract-java.lang.String-) | Estrae la voce nel file specificato. |
| [extract(String path, String password)](#extract-java.lang.String-java.lang.String-) | Estrae la voce nel file specificato usando una password opzionale. |
| [getCompressedSize()](#getCompressedSize--) | Restituisce la dimensione compressa dei dati della voce in byte. |
| [getLength()](#getLength--) | Restituisce la lunghezza decompressa di questa voce. |
| [getName()](#getName--) | Restituisce il nome della voce memorizzato nell'archivio. |
| [getUncompressedSize()](#getUncompressedSize--) | Restituisce la dimensione decompressa dei dati della voce in byte. |
| [isDirectory()](#isDirectory--) | Restituisce se questa voce rappresenta una directory. |
| [open()](#open--) | Apre la voce e fornisce un flusso contenente dati decompressi. |
| [open(String password)](#open-java.lang.String-) | Apre la voce e fornisce un flusso contenente dati decompressi. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Estrae la voce in un flusso scrivibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | flusso di destinazione |

### extract(OutputStream destination, String password) {#extract-java.io.OutputStream-java.lang.String-}
```
public final void extract(OutputStream destination, String password)
```


Estrae la voce in un flusso scrivibile usando una password opzionale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinazione | java.io.OutputStream | flusso di destinazione |
| password | java.lang.String | password opzionale per questa voce |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Estrae la voce nel file specificato. Un file esistente viene sovrascritto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | percorso del file di destinazione |

**Returns:**
java.io.File - file estratto
### extract(String path, String password) {#extract-java.lang.String-java.lang.String-}
```
public final File extract(String path, String password)
```


Estrae la voce nel file specificato usando una password opzionale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | percorso del file di destinazione |
| password | java.lang.String | password opzionale per questa voce |

**Returns:**
java.io.File - file estratto
### getCompressedSize() {#getCompressedSize--}
```
public final long getCompressedSize()
```


Restituisce la dimensione compressa dei dati della voce in byte.

**Returns:**
long - dimensione compressa in byte
### getLength() {#getLength--}
```
public final Long getLength()
```


Restituisce la lunghezza decompressa di questa voce.

**Returns:**
java.lang.Long - lunghezza non compressa in byte
### getName() {#getName--}
```
public final String getName()
```


Restituisce il nome della voce memorizzato nell'archivio.

**Returns:**
java.lang.String - nome della voce
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Restituisce la dimensione decompressa dei dati della voce in byte.

**Returns:**
long - dimensione non compressa in byte
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Restituisce se questa voce rappresenta una directory.

**Returns:**
boolean - `true` per una voce di directory
### open() {#open--}
```
public final InputStream open()
```


Apre la voce e fornisce un flusso contenente dati decompressi.

**Returns:**
java.io.InputStream - flusso contenente i dati della voce decompressa
### open(String password) {#open-java.lang.String-}
```
public final InputStream open(String password)
```


Apre la voce e fornisce un flusso contenente dati decompressi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| password | java.lang.String | password opzionale per questa voce |

**Returns:**
java.io.InputStream - flusso contenente i dati della voce decompressa
