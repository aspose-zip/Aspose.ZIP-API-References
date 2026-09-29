---
title: "WimEntry"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un singolo file o directory all'interno di un'immagine wim."
type: docs
weight: 132
url: /it/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Rappresenta un singolo file o directory all'interno di un'immagine wim.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Ottiene i nomi dei flussi di dati alternativi per il file o la directory. |
| [getArchive()](#getArchive--) | Ottiene l'archivio a cui appartiene la voce. |
| [getChangeTime()](#getChangeTime--) | Ottiene l'ultima volta in cui il file o la directory è stato modificato. |
| [getCreationTime()](#getCreationTime--) | Ottiene l'ora di creazione del file o della directory. |
| [getFileAttributes()](#getFileAttributes--) | Ottiene gli attributi del file o della directory. |
| [getFullPath()](#getFullPath--) | Ottiene il percorso completo della voce all'interno dell'immagine. |
| [getHardLink()](#getHardLink--) | Ottiene l'ID del collegamento fisso del file o della directory. |
| [getImage()](#getImage--) | Ottiene l'immagine a cui appartiene la voce. |
| [getLastAccessTime()](#getLastAccessTime--) | Ottiene l'ultima ora di accesso del file o della directory. |
| [getLastWriteTime()](#getLastWriteTime--) | Ottiene l'ora di modifica del file o della directory. |
| [getModificationTime()](#getModificationTime--) | Ottiene l'ora di modifica del file o della directory. |
| [getName()](#getName--) | Ottiene il nome della voce all'interno dell'immagine. |
| [getParent()](#getParent--) | Ottiene la directory padre a cui appartiene la voce. |
| [getShortName()](#getShortName--) | Ottiene il nome breve della voce all'interno dell'immagine. |
| [hasHardLinks()](#hasHardLinks--) | Ottiene se il file o la directory è conosciuto con altri nomi. |
| [isDirectory()](#isDirectory--) | Ottiene un valore che indica se la voce rappresenta una directory. |
| [toString()](#toString--) | Restituisce la rappresentazione stringa dell'istanza della classe [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Ottiene i nomi dei flussi di dati alternativi per il file o la directory.

**Returns:**
java.lang.String[] - i nomi dei flussi di dati alternativi per il file o la directory
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Ottiene l'archivio a cui appartiene la voce.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Ottiene l'ultima volta in cui il file o la directory è stato modificato.

**Returns:**
java.util.Date - l'ultima volta in cui il file o la directory è stato modificato
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Ottiene l'ora di creazione del file o della directory.

**Returns:**
java.util.Date - il tempo di creazione del file o della directory
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Ottiene gli attributi del file o della directory.

**Returns:**
int - gli attributi del file o della directory
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Ottiene il percorso completo della voce all'interno dell'immagine.

**Returns:**
java.lang.String - il percorso completo della voce all'interno dell'immagine
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Ottiene l'ID del collegamento fisso del file o della directory.

**Returns:**
long - l'ID hardlink del file o della directory
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Ottiene l'immagine a cui appartiene la voce.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Ottiene l'ultima ora di accesso del file o della directory.

**Returns:**
java.util.Date - l'ultimo momento di accesso del file o della directory
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Ottiene l'ora di modifica del file o della directory.

**Returns:**
java.util.Date - il tempo di modifica del file o della directory
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Ottiene l'ora di modifica del file o della directory.

**Returns:**
java.util.Date - il tempo di modifica del file o della directory
### getName() {#getName--}
```
public final String getName()
```


Ottiene il nome della voce all'interno dell'immagine.

**Returns:**
java.lang.String - il nome della voce all'interno dell'immagine
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Ottiene la directory padre a cui appartiene la voce.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Ottiene il nome breve della voce all'interno dell'immagine.

**Returns:**
java.lang.String - il nome breve della voce all'interno dell'immagine
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Ottiene se il file o la directory è conosciuto con altri nomi.

**Returns:**
boolean - se il file o la directory è noto con altri nomi
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Ottiene un valore che indica se la voce rappresenta una directory.

**Returns:**
boolean - un valore che indica se la voce rappresenta una directory
### toString() {#toString--}
```
public String toString()
```


Restituisce la rappresentazione stringa dell'istanza della classe [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - rappresentazione stringa di questo oggetto
