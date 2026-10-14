---
title: "WimArchive"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Questa classe rappresenta un file di archivio wim."
type: docs
weight: 130
url: /it/java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive implements IArchive, AutoCloseable
```

Questa classe rappresenta un file di archivio wim.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Inizializza una nuova istanza della classe [WimArchive](../../com.aspose.zip/wimarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)](#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-) | Inizializza una nuova istanza della classe [WimArchive](../../com.aspose.zip/wimarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Inizializza una nuova istanza della classe [WimArchive](../../com.aspose.zip/wimarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
| [WimArchive(String path, WimLoadOptions loadOptions)](#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-) | Inizializza una nuova istanza della classe [WimArchive](../../com.aspose.zip/wimarchive) e compone un elenco di voci che può essere estratto dall'archivio. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Estrae l'archivio nel file specificato dal percorso. |
| [getBootImageIndex()](#getBootImageIndex--) | Restituisce l'indice (basato su zero) dell'immagine avviabile. |
| [getEntries()](#getEntries--) | Restituisce le voci di tipo [WimEntry](../../com.aspose.zip/wimentry) che costituiscono l'archivio. |
| [getFileEntries()](#getFileEntries--) | Restituisce le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio wim. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Restituisce la versione del formato file. |
| [getFormat()](#getFormat--) | Ottiene il formato dell'archivio. |
| [getGuid()](#getGuid--) | Restituisce l'UUID identificativo per l'archivio. |
| [getImages()](#getImages--) | Restituisce le voci di tipo [WimImage](../../com.aspose.zip/wimimage) che costituiscono l'archivio. |
| [getManifest()](#getManifest--) | Restituisce il manifesto incorporato che descrive il file e le immagini contenute. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Inizializza una nuova istanza della classe [WimArchive](../../com.aspose.zip/wimarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```

``````

try (WimArchive archive = new WimArchive(new FileInputStream(\"archive.wim\"))) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
} catch (IOException ex) {
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(InputStream sourceStream, WimLoadOptions loadOptions) {#WimArchive-java.io.InputStream-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(InputStream sourceStream, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

Questo costruttore non estrae alcuna voce. Vedere il metodo [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) per l'estrazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceStream | java.io.InputStream | la sorgente dell'archivio |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opzioni per caricare l'archivio esistente. |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Inizializza una nuova istanza della classe [WimArchive](../../com.aspose.zip/wimarchive) e compone un elenco di voci che può essere estratto dall'archivio.

Il seguente esempio mostra come estrarre tutte le voci in una directory.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
}
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### WimArchive(String path, WimLoadOptions loadOptions) {#WimArchive-java.lang.String-com.aspose.zip.WimLoadOptions-}
```
public WimArchive(String path, WimLoadOptions loadOptions)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

``````

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

Questo costruttore non estrae alcuna voce. Vedere il metodo [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\\#open--) per l'estrazione.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| path | java.lang.String | il percorso del file di archivio |
| loadOptions | [WimLoadOptions](../../com.aspose.zip/wimloadoptions) | Opzioni per caricare l'archivio esistente. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Estrae l'archivio nel file specificato dal percorso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| destinationDirectory | java.lang.String | il percorso della directory in cui posizionare i file estratti |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Restituisce l'indice (basato su zero) dell'immagine avviabile.

**Returns:**
int - l'indice (basato su zero) dell'immagine avviabile
### getEntries() {#getEntries--}
```
public final List<WimEntry> getEntries()
```


Restituisce le voci di tipo [WimEntry](../../com.aspose.zip/wimentry) che costituiscono l'archivio.

**Returns:**
java.util.List&lt;com.aspose.zip.WimEntry&gt; - voci che costituiscono l'archivio
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Restituisce le voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio wim.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - voci di tipo [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) che costituiscono l'archivio wim
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Restituisce la versione del formato file.

**Returns:**
int - la versione del formato file
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Ottiene il formato dell'archivio.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Restituisce l'UUID identificativo per l'archivio.

**Returns:**
java.util.UUID - l'UUID identificativo per l'archivio
### getImages() {#getImages--}
```
public final List<WimImage> getImages()
```


Restituisce le voci di tipo [WimImage](../../com.aspose.zip/wimimage) che costituiscono l'archivio.

**Returns:**
java.util.List&lt;com.aspose.zip.WimImage&gt; - voci di tipo [WimImage](../../com.aspose.zip/wimimage) che costituiscono l'archivio
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Restituisce il manifesto incorporato che descrive il file e le immagini contenute.

**Returns:**
java.lang.String - il manifesto incorporato che descrive il file e le immagini contenute
