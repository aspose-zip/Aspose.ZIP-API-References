---
title: ZArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents Z compress archive file.
type: docs
weight: 108
url: /java/com.aspose.zip/zarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class ZArchive implements IArchiveFileEntry, IArchive, AutoCloseable
```

This class represents Z (compress) archive file. Use it to compose or extract Z archives.

See [Z Compressed File Format ][Z Compressed File Format]


[Z Compressed File Format]: https://docs.fileformat.com/compression/z/
## Constructors

| Constructor | Description |
| --- | --- |
| [ZArchive()](#ZArchive--) | Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for compressing. |
| [ZArchive(InputStream source)](#ZArchive-java.io.InputStream-) | Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing. |
| [ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)](#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-) | Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing. |
| [ZArchive(String path)](#ZArchive-java.lang.String-) | Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing. |
| [ZArchive(String path, ZArchiveLoadOptions loadOptions)](#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-) | Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(File file)](#extract-java.io.File-) | Extracts Z archive to a file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts Z archive to a stream. |
| [extract(String path)](#extract-java.lang.String-) | Extracts Z archive to a file by path. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts content of the archive to the directory provided. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive. |
| [getLength()](#getLength--) | Get length of the entry in bytes. |
| [getName()](#getName--) | Gets the name of the entry within archive. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves Z archive to the stream provided. |
| [save(OutputStream output, ZArchiveSaveOptions settings)](#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-) | Saves Z archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves Z archive to destination file provided. |
| [save(String destinationFileName, ZArchiveSaveOptions settings)](#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-) | Saves Z archive to destination file provided. |
| [setSource(File file)](#setSource-java.io.File-) | Sets the content to be compressed within the archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Sets the content to be compressed within the archive. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Sets the content to be compressed within the archive. |
### ZArchive() {#ZArchive--}
```
public ZArchive()
```


Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for compressing.

### ZArchive(InputStream source) {#ZArchive-java.io.InputStream-}
```
public ZArchive(InputStream source)
```


Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the source of the archive |

### ZArchive(InputStream source, ZArchiveLoadOptions loadOptions) {#ZArchive-java.io.InputStream-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(InputStream source, ZArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(OutputStream)](../../com.aspose.zip/zarchive\#extract-OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the source of the archive |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | the options to load archive with |

### ZArchive(String path) {#ZArchive-java.lang.String-}
```
public ZArchive(String path)
```


Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### ZArchive(String path, ZArchiveLoadOptions loadOptions) {#ZArchive-java.lang.String-com.aspose.zip.ZArchiveLoadOptions-}
```
public ZArchive(String path, ZArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [ZArchive](../../com.aspose.zip/zarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(String)](../../com.aspose.zip/zarchive\#extract-String-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |
| loadOptions | [ZArchiveLoadOptions](../../com.aspose.zip/zarchiveloadoptions) | the options to load archive with |

### close() {#close--}
```
public void close()
```




### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts Z archive to a file.

```

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (ZArchive archive = new ZArchive(zFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
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


Extracts Z archive to a stream.

```

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (ZArchive archive = new ZArchive(zFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
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


Extracts Z archive to a file by path.

```

     try (FileInputStream zFile = new FileInputStream("sourceFileName")) {
         try (ZArchive archive = new ZArchive(zFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to file which will store decompressed data |

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
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the Z archive
### getLength() {#getLength--}
```
public final Long getLength()
```


Get length of the entry in bytes.

**Returns:**
java.lang.Long - the length of the entry in bytes
### getName() {#getName--}
```
public final String getName()
```


Gets the name of the entry within archive.

**Returns:**
java.lang.String - the name of the entry within archive
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves Z archive to the stream provided.

```

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(OutputStream output, ZArchiveSaveOptions settings) {#save-java.io.OutputStream-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(OutputStream output, ZArchiveSaveOptions settings)
```


Saves Z archive to the stream provided.

```

     try (FileOutputStream zFile = new FileOutputStream("data.bin.Z")) {
         try (ZArchive archive = new ZArchive()) {
             archive.setSource("data.bin");
             archive.save(zFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves Z archive to destination file provided.

```

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |

### save(String destinationFileName, ZArchiveSaveOptions settings) {#save-java.lang.String-com.aspose.zip.ZArchiveSaveOptions-}
```
public final void save(String destinationFileName, ZArchiveSaveOptions settings)
```


Saves Z archive to destination file provided.

```

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten |
| settings | [ZArchiveSaveOptions](../../com.aspose.zip/zarchivesaveoptions) | the settings for archive composition |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | the file info which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

     try (ZArchive archive = new ZArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.Z");
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

     try (ZArchive archive = new ZArchive()) {
         archive.setSource("data.bin");
         archive.save("data.bin.Z");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | the path to the file which will be opened as input stream |

