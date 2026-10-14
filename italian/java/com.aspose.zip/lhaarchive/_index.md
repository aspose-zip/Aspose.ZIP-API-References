---
title: "LhaArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file archivio LHA .lzh."
type: docs
weight: 75
url: /it/java/com.aspose.zip/lhaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LhaArchive implements IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio LHA (.lzh).

Sono supportati solo i seguenti metodi di compressione:

| ------ | --------------------------------------------- |
| Metodo | Spiegazione                                   |
| lh0    | Non compresso                                  |
| lh4    | 8 KiB dizionario a scorrimento e Huffman statico   |
| lh5    | 16 KiB dizionario a scorrimento e Huffman statico  |
| lh6    | 64 KiB dizionario a scorrimento e Huffman statico  |
| lh7    | 128 KiB dizionario a scorrimento e Huffman statico |
| lhx    | 1 Mib dizionario a scorrimento e Huffman statico   |
| lhd    | Directory                                     |
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LhaArchive(InputStream sourceStream)](#LhaArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)](#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-) | Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [LhaArchive(String path)](#LhaArchive-java.lang.String-) | Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [LhaArchive(String path, LhaLoadOptions loadOptions)](#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-) | Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file e le directory presenti nell'archivio nella directory fornita. |
| [getEntries()](#getEntries--) | Restituisce le voci file di tipo [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) che costituiscono l'archivio. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
### LhaArchive(InputStream sourceStream) {#LhaArchive-java.io.InputStream-}
```
public LhaArchive(InputStream sourceStream)
```


Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Questo costruttore non decomprime alcuna voce. Vedi il metodo [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la sorgente dell'archivio |

### LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions) {#LhaArchive-java.io.InputStream-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(InputStream sourceStream, LhaLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Questo costruttore non decomprime alcuna voce. Vedi il metodo [LhaArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lhaarchiveentry\#extract-OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la sorgente dell'archivio |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opzioni per caricare l'archivio esistente. |

### LhaArchive(String path) {#LhaArchive-java.lang.String-}
```
public LhaArchive(String path)
```


Inizializza una nuova istanza della classe [LhaArchive](../../com.aspose.zip/lhaarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio estrae un archivio, quindi decomprime la prima voce in un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LhaArchive archive = new LhaArchive("sample.lzh")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the fully qualified or the relative path to the archive file |

### LhaArchive(String path, LhaLoadOptions loadOptions) {#LhaArchive-java.lang.String-com.aspose.zip.LhaLoadOptions-}
```
public LhaArchive(String path, LhaLoadOptions loadOptions)
```


Initializes a new instance of the [LhaArchive](../../com.aspose.zip/lhaarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LhaArchive archive = new LhaArchive("sample.lzh")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Questo costruttore non decomprime alcuna voce. Vedi il metodo [ArchiveEntry.extract(OutputStream)](../../com.aspose.zip/archiveentry\#extract-OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso completamente qualificato o relativo al file di archivio |
| loadOptions | [LhaLoadOptions](../../com.aspose.zip/lhaloadoptions) | Opzioni per caricare l'archivio esistente. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae tutti i file e le directory presenti nell'archivio nella directory fornita.

```

``````

try (LhaArchive archive = new LhaArchive("archive.lzh")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getEntries() {#getEntries--}
```
public final List<LhaArchiveEntry> getEntries()
```


Gets file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LhaArchiveEntry&gt; - file entries of [LhaArchiveEntry](../../com.aspose.zip/lhaarchiveentry) type constituting the archive
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
