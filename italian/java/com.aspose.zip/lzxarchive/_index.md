---
title: "LzxArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio LZX .lzx."
type: docs
weight: 89
url: /it/java/com.aspose.zip/lzxarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class LzxArchive implements IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio LZX (.lzx).
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LzxArchive(InputStream extractionSource)](#LzxArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)](#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-) | Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [LzxArchive(String path)](#LzxArchive-java.lang.String-) | Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [LzxArchive(String path, LzxLoadOptions loadOptions)](#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-) | Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutti i file e le directory presenti nell'archivio nella directory fornita. |
| [getEntries()](#getEntries--) | Ottiene le voci file di tipo [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) che costituiscono l'archivio. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
### LzxArchive(InputStream extractionSource) {#LzxArchive-java.io.InputStream-}
```
public LzxArchive(InputStream extractionSource)
```


Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Questo costruttore non decomprime alcuna voce. Vedi il metodo [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) per la decompressione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extractionSource | java.io.InputStream | La sorgente dell'archivio. |

### LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions) {#LzxArchive-java.io.InputStream-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(InputStream extractionSource, LzxLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Questo costruttore non decomprime alcuna voce. Vedi il metodo [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) per la decompressione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extractionSource | java.io.InputStream | La sorgente dell'archivio. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opzioni per caricare l'archivio esistente. |

### LzxArchive(String path) {#LzxArchive-java.lang.String-}
```
public LzxArchive(String path)
```


Inizializza una nuova istanza della classe [LzxArchive](../../com.aspose.zip/lzxarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio estrae un archivio, quindi decomprime la prima voce in un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (LzxArchive archive = new LzxArchive("sample.lzx")) {
archive.getEntries().get(0).extract(extracted);
}
 
```

This constructor does not decompress any entry. See [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### LzxArchive(String path, LzxLoadOptions loadOptions) {#LzxArchive-java.lang.String-com.aspose.zip.LzxLoadOptions-}
```
public LzxArchive(String path, LzxLoadOptions loadOptions)
```


Initializes a new instance of the [LzxArchive](../../com.aspose.zip/lzxarchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (LzxArchive archive = new LzxArchive("sample.lzx")) {
         archive.getEntries().get(0).extract(extracted);
     }
 
```

Questo costruttore non decomprime alcuna voce. Vedi il metodo [LzxArchiveEntry.extract(OutputStream)](../../com.aspose.zip/lzxarchiveentry\#extract-OutputStream-) per la decompressione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | Il percorso completo o relativo al file dell'archivio. |
| loadOptions | [LzxLoadOptions](../../com.aspose.zip/lzxloadoptions) | Opzioni per caricare l'archivio esistente. |

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

try (LzxArchive archive = new LzxArchive("archive.lzx")) {
archive.extractToDirectory("C:/extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getEntries() {#getEntries--}
```
public final List<LzxArchiveEntry> getEntries()
```


Gets file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.LzxArchiveEntry&gt; - file entries of [LzxArchiveEntry](../../com.aspose.zip/lzxarchiveentry) type constituting the archive.
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
