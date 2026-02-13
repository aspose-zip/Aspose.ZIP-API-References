---
title: ArjArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents an ARJ archive file.
type: docs
weight: 21
url: /java/com.aspose.zip/arjarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ArjArchive implements IArchive, AutoCloseable
```

This class represents an ARJ archive file.

Only the following compression methods are supported:

    | ------ | ------------------------------------------------------------ |
    | Method | Explanation                                                  |
    | 0      | Uncompressed                                                 |
    | 1      | Combination of LZ77 and adaptive Huffman coding. Best ratio. |
    | 2      | Combination of LZ77 and adaptive Huffman coding.             |
    | 3      | Combination of LZ77 and adaptive Huffman coding. Best speed. |
## Constructors

| Constructor | Description |
| --- | --- |
| [ArjArchive(InputStream extractionSource)](#ArjArchive-java.io.InputStream-) | Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive. |
| [ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)](#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-) | Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive. |
| [ArjArchive(String path)](#ArjArchive-java.lang.String-) | Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive. |
| [ArjArchive(String path, ArjLoadOptions loadOptions)](#ArjArchive-java.lang.String-com.aspose.zip.ArjLoadOptions-) | Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts all entries to the specified directory. |
| [getCommentary()](#getCommentary--) | Gets the commentary. |
| [getEntries()](#getEntries--) | Gets entries of [ArjEntryPlain](../../com.aspose.zip/arjentryplain) type constituting the ARJ archive. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive. |
| [getFormat()](#getFormat--) | Gets the archive format. |
| [getName()](#getName--) | Gets the original name. |
### ArjArchive(InputStream extractionSource) {#ArjArchive-java.io.InputStream-}
```
public ArjArchive(InputStream extractionSource)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

This constructor does not decompress any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extractionSource | java.io.InputStream | the source of the archive |

### ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions) {#ArjArchive-java.io.InputStream-com.aspose.zip.ArjLoadOptions-}
```
public ArjArchive(InputStream extractionSource, ArjLoadOptions loadOptions)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

This constructor does not decompress any entry. See [ArjEntryPlain.extract(java.io.OutputStream)](../../com.aspose.zip/arjentryplain\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extractionSource | java.io.InputStream | the source of the archive |
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Options to load existing archive with. |

### ArjArchive(String path) {#ArjArchive-java.lang.String-}
```
public ArjArchive(String path)
```


Initializes a new instance of the [ArjArchive](../../com.aspose.zip/arjarchive) class and composes an entry list can be extracted from the archive.

The following example shows how to extract all the entries to a directory.

```

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
| loadOptions | [ArjLoadOptions](../../com.aspose.zip/arjloadoptions) | Options to load existing archive with. |

### close() {#close--}
```
public void close()
```




### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all entries to the specified directory.

The following example shows how to extract all entries to a directory:

```

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
