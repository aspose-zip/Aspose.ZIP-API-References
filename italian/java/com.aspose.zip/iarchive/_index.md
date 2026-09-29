---
title: "IArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa interfaccia rappresenta un archivio."
type: docs
weight: 161
url: /it/java/com.aspose.zip/iarchive/
---

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public interface IArchive extends AutoCloseable
```

Questa interfaccia rappresenta un archivio.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file dell'archivio nella directory fornita. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
### close() {#close--}
```
public abstract void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public abstract void extractToDirectory(String destinationDirectory)
```


Estrae tutti i file dell'archivio nella directory fornita.

Se la directory non esiste, verrà creata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | java.lang.String | Il percorso della directory in cui posizionare i file estratti. |

### getFileEntries() {#getFileEntries--}
```
public abstract Iterable<IArchiveFileEntry> getFileEntries()
```


Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio.

Gli archivi solo per compressione, come gzip, bzip2, lzip, lzma, lz4, xz, z, consistono in un unico record - l'archivio stesso.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio.
### getFormat() {#getFormat--}
```
public abstract ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
