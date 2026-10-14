---
title: "RarArchive"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Cette classe représente un fichier d'archive RAR."
type: docs
weight: 97
url: /fr/java/com.aspose.zip/rararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class RarArchive implements IArchive, AutoCloseable
```

Cette classe représente un fichier d'archive RAR. Utilisez-la pour extraire des archives RAR.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [RarArchive(String path)](#RarArchive-java.lang.String-) | Initialise une nouvelle instance de la classe [RarArchive](../../com.aspose.zip/rararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [RarArchive(String path, RarArchiveLoadOptions loadOptions)](#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [RarArchive](../../com.aspose.zip/rararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [RarArchive(InputStream sourceStream)](#RarArchive-java.io.InputStream-) | Initialise une nouvelle instance de la classe [RarArchive](../../com.aspose.zip/rararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
| [RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)](#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-) | Initialise une nouvelle instance de la classe [RarArchive](../../com.aspose.zip/rararchive) et compose une liste d'entrées pouvant être extraites de l'archive. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [close()](#close--) | \\{@inheritDoc\\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extrait tous les fichiers de l'archive vers le répertoire fourni. |
| [getEntries()](#getEntries--) | Obtient les entrées de type [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) constituant l'archive rar. |
| [getFileEntries()](#getFileEntries--) | Obtient les entrées de type [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) constituant l'archive rar. |
| [getFormat()](#getFormat--) | Obtient le format de l'archive. |
### RarArchive(String path) {#RarArchive-java.lang.String-}
```
public RarArchive(String path)
```


Initialise une nouvelle instance de la classe [RarArchive](../../com.aspose.zip/rararchive) et compose une liste d'entrées pouvant être extraites de l'archive.

L'exemple suivant extrait une archive, puis décompresse la première entrée vers un `MemoryStream`.

```

``````

ByteArrayOutputStream extracted = new ByteArrayOutputStream();
try (RarArchive archive = new RarArchive("data.rar")) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
} catch (IOException ex) {
}
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### RarArchive(String path, RarArchiveLoadOptions loadOptions) {#RarArchive-java.lang.String-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(String path, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.

The following example extracts an archive, then decompress first entry to a `MemoryStream`.

```

``````

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     try (RarArchive archive = new RarArchive("data.rar")) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Le chemin complet ou relatif vers le fichier d’archive. |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | Options pour charger une archive existante. |

### RarArchive(InputStream sourceStream) {#RarArchive-java.io.InputStream-}
```
public RarArchive(InputStream sourceStream)
```


Initialise une nouvelle instance de la classe [RarArchive](../../com.aspose.zip/rararchive) et compose une liste d'entrées pouvant être extraites de l'archive.


L'exemple suivant déchiffre et décompresse la première entrée vers un `MemoryStream`.

```

``````

try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
ByteArrayOutputStream extracted = new ByteArrayOutputStream();
RarArchiveLoadOptions options = new RarArchiveLoadOptions();
options.setDecryptionPassword("p@s$");
try (RarArchive archive = new RarArchive(fs, options)) {
try (InputStream decompressed = archive.getEntries().get(0).open()) {
byte[] b = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
extracted.write(b, 0, bytesRead);
}
}
} catch (IOException ex) {
}
 
```

This constructor does not decompress any entry. See [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions) {#RarArchive-java.io.InputStream-com.aspose.zip.RarArchiveLoadOptions-}
```
public RarArchive(InputStream sourceStream, RarArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [RarArchive](../../com.aspose.zip/rararchive) class and composes an entry list can be extracted from the archive.


The following example decipher and decompress first entry to a `MemoryStream`.

```

``````

     try (FileInputStream fs = new FileInputStream("encrypted.rar")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         RarArchiveLoadOptions options = new RarArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (RarArchive archive = new RarArchive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 < (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

Ce constructeur ne décompresse aucune entrée. Voir la méthode [RarArchiveEntry.open()](../../com.aspose.zip/rararchiveentry\#open--) pour la décompression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | La source de l’archive. |
| loadOptions | [RarArchiveLoadOptions](../../com.aspose.zip/rararchiveloadoptions) | Options pour charger une archive existante. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extrait tous les fichiers de l'archive vers le répertoire fourni.

```

``````

try (RarArchive archive = new RarArchive("archive.rar")) {
archive.extractToDirectory(\"C:\\\\extracted\");
}
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<RarArchiveEntry> getEntries()
```


Gets entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.

**Returns:**
java.util.List&lt;com.aspose.zip.RarArchiveEntry&gt; - entries of [RarArchiveEntry](../../com.aspose.zip/rararchiveentry) type constituting the rar archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the rar archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
