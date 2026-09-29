---
title: "ArjArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio ARJ."
type: docs
weight: 37
url: /it/java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio ARJ.

Sono supportati solo i seguenti metodi di compressione:

| ------ | ------------------------------------------------------------ |
| Metodo | Spiegazione                                                  |
| 0      | Non compresso                                                 |
| 1      | Combinazione di LZ77 e codifica Huffman adattiva. Rapporto migliore. |
| 2      | Combinazione di LZ77 e codifica Huffman adattiva.             |
| 3      | Combinazione di LZ77 e codifica Huffman adattiva. Velocità migliore. |
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae tutte le voci nella directory specificata. |
| [getCommentary()](#getCommentary--) | Ottiene il commento. |
| [getEntries()](#getEntries--) | Ottiene le voci di tipo [ArjEntryPlain](../../com.aspose.zip/arjentryplain) che costituiscono l'archivio ARJ. |
| [getFileEntries()](#getFileEntries--) | Ottiene le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getName()](#getName--) | Ottiene il nome originale. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Questo costruttore non decomprime alcuna voce. Vedi il metodo [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extractionSource | java.io.InputStream | la sorgente dell'archivio |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Questo costruttore non decomprime alcuna voce. Vedi il metodo [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| extractionSource | java.io.InputStream | la sorgente dell'archivio |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Opzioni per caricare l'archivio esistente. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Inizializza una nuova istanza della classe [ArjArchive](../../com.aspose.zip/arjarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```

``````

try (ArjArchive archive = new ArjArchive("archive.arj")) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### ArjArchive(String path, ArjLoadOptions loadOptions) {#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(String path, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

``````

     try (ArjArchive archive = new ArjArchive("archive.arj")) {
         archive.extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Questo costruttore non estrae alcuna voce. Vedi il metodo [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) per decomprimere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Opzioni per caricare l'archivio esistente. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae tutte le voci nella directory specificata.

Il seguente esempio mostra come estrarre tutte le voci in una directory:

```

``````

try (ArjArchive archive = new ArjArchive(new FileInputStream("archive.arj"))) {
archive.extractToDirectory("C:\\extracted");
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the directory to extract the entries to |

### getCommentary() {#getCommentary--}
```
public final String getCommentary()
```


Gets the commentary.

**Returns:**
java.lang.String - the commentary.
### getEntries() {#getEntries--}
```
public final List<ArjEntryPlain> getEntries()
```


Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArjEntryPlain&gt; - entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive.
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
### getName() {#getName--}
```
public final String getName()
```


Gets the original name.

**Returns:**
java.lang.String - the original name.
