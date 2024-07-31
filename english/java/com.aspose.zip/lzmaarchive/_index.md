---
title: LzmaArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents LZMA archive file.
type: docs
weight: 42
url: /java/com.aspose.zip/lzmaarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class LzmaArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

This class represents LZMA archive file. Use it to compose or extract LZMA archives.
## Constructors

| Constructor | Description |
| --- | --- |
| [LzmaArchive()](#LzmaArchive--) | Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class and composes the archive in lzma format. |
| [LzmaArchive(LzmaArchiveSettings settings)](#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-) | Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class and composes the archive in lzma format. |
| [LzmaArchive(InputStream source)](#LzmaArchive-java.io.InputStream-) | Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class prepared for decompressing. |
| [LzmaArchive(String path)](#LzmaArchive-java.lang.String-) | Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class prepared for decompressing. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extracts lzma archive to a file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts lzma archive to a stream. |
| [extract(String path)](#extract-java.lang.String-) | Extracts lzma archive to a file by path. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts content of the archive to the directory provided. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzma archive. |
| [getLength()](#getLength--) | Gets length. |
| [getName()](#getName--) | The name of original file. |
| [save(File destination)](#save-java.io.File-) | Saves lzma archive to destination file provided. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves lzma archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves lzma archive to destination file provided. |
| [setSource(File file)](#setSource-java.io.File-) | Sets the content to be compressed within the archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Sets the content to be compressed within the archive. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Sets the content to be compressed within the archive. |
### LzmaArchive() {#LzmaArchive--}
```
public LzmaArchive()
```


Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class and composes the archive in lzma format.

### LzmaArchive(LzmaArchiveSettings settings) {#LzmaArchive-com.aspose.zip.LzmaArchiveSettings-}
```
public LzmaArchive(LzmaArchiveSettings settings)
```


Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class and composes the archive in lzma format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [LzmaArchiveSettings](../../com.aspose.zip/lzmaarchivesettings) | set of setting particular lzma archive |

### LzmaArchive(InputStream source) {#LzmaArchive-java.io.InputStream-}
```
public LzmaArchive(InputStream source)
```


Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the source of the archive |

### LzmaArchive(String path) {#LzmaArchive-java.lang.String-}
```
public LzmaArchive(String path)
```


Initializes a new instance of the [LzmaArchive](../../com.aspose.zip/lzmaarchive) class prepared for decompressing.

```

     try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
         try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
             try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/lzmaarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts lzma archive to a file.

```

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts lzma archive to a stream.

```

     try (FileInputStream sourceLzmaFile = new FileInputStream(sourceFileName)) {
         try (FileOutputStream extractedFile = new FileOutputStream(extractedFileName)) {
             try (LzmaArchive archive = new LzmaArchive(sourceLzmaFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | the stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts lzma archive to a file by path.

```

     try (FileInputStream lzmaFile = new FileInputStream(sourceFileName)) {
         try (LzmaArchive archive = new LzmaArchive(lzmaFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the file which will store decompressed data |

**Returns:**
java.io.File - the file info of the extracted file
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzma archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the lzma archive.
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets length.

**Returns:**
java.lang.Long - length
### getName() {#getName--}
```
public final String getName()
```


The name of original file.

**Returns:**
java.lang.String - the name of the original file
### save(File destination) {#save-java.io.File-}
```
public final void save(File destination)
```


Saves lzma archive to destination file provided.

```

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(new File("archive.lzma"));
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.File | the file which will be opened as destination stream |

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves lzma archive to the stream provided.

```

     try (FileOutputStream lzmaFile = new FileOutputStream("archive.lzma")) {
         try (LzmaArchive archive = new LzmaArchive()) {
             archive.setSource("data.bin");
             archive.save(lzmaFile);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves lzma archive to destination file provided.

```

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.lzma");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the input stream for the archive |

### setSource(String sourcePath) {#setSource-java.lang.String-}
```
public final void setSource(String sourcePath)
```


Sets the content to be compressed within the archive.

```

     try (LzmaArchive archive = new LzmaArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.lzma");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | path to file which will be opened as input stream |

