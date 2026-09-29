---
title: "AlzArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta un file di archivio ALZ."
type: docs
weight: 11
url: /it/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Rappresenta un file di archivio ALZ. Usa questa classe per ispezionare ed estrarre archivi ALZ.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Inizializza un archivio ALZ da un flusso. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Inizializza un archivio ALZ da un flusso usando le opzioni di caricamento fornite. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Inizializza un archivio ALZ da un percorso file. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Inizializza un archivio ALZ da un percorso file usando le opzioni di caricamento fornite. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | Rilascia le risorse detenute da questo archivio. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file e le directory nella directory fornita. |
| [getEntries()](#getEntries--) | Ottiene le voci che costituiscono questo archivio. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci tramite l'interfaccia comune dell'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Inizializza un archivio ALZ da un flusso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Flusso di archivio ALZ; deve supportare lettura e ricerca |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Inizializza un archivio ALZ da un flusso usando le opzioni di caricamento fornite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Flusso di archivio ALZ; deve supportare lettura e ricerca |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opzioni usate per caricare l'archivio |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Inizializza un archivio ALZ da un percorso file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | percorso a un archivio ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Inizializza un archivio ALZ da un percorso file usando le opzioni di caricamento fornite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | percorso a un archivio ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | opzioni usate per caricare l'archivio |

### close() {#close--}
```
public void close()
```


Rilascia le risorse detenute da questo archivio.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae tutti i file e le directory nella directory fornita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | java.lang.String | directory di destinazione; viene creata se necessario |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Ottiene le voci che costituiscono questo archivio.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - elenco immutabile di voci ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Ottiene le voci tramite l'interfaccia comune dell'archivio.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci dell'archivio
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
