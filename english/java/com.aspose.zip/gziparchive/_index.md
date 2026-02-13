---
title: GzipArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents a gzip archive file.
type: docs
weight: 52
url: /java/com.aspose.zip/gziparchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), [com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), java.lang.AutoCloseable
```
public class GzipArchive implements IArchive, IArchiveFileEntry, AutoCloseable
```

This class represents a gzip archive file. Use it to compose or extract gzip archives.

Gzip compression algorithm is based on the DEFLATE algorithm, which is a combination of LZ77 and Huffman coding.
## Constructors

| Constructor | Description |
| --- | --- |
| [GzipArchive()](#GzipArchive--) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for compressing. |
| [GzipArchive(InputStream sourceStream)](#GzipArchive-java.io.InputStream-) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing. |
| [GzipArchive(InputStream sourceStream, boolean parseHeader)](#GzipArchive-java.io.InputStream-boolean-) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing. |
| [GzipArchive(InputStream sourceStream, GzipLoadOptions options)](#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing. |
| [GzipArchive(String path, GzipLoadOptions options)](#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing. |
| [GzipArchive(String path)](#GzipArchive-java.lang.String-) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class. |
| [GzipArchive(String path, boolean parseHeader)](#GzipArchive-java.lang.String-boolean-) | Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the archive to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the archive to the file by path. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts content of the archive to the directory provided. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the gzip archive. |
| [getFormat()](#getFormat--) | Gets the archive format. |
| [getLength()](#getLength--) | Gets size of an original file. |
| [getName()](#getName--) | The name of the original file. |
| [getUncompressedSize()](#getUncompressedSize--) | Gets size of an original file. |
| [open()](#open--) | Opens the archive for extraction and provides a stream with archive content. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Saves archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves archive to the destination file provided. |
| [setSource(TarArchive tarArchive)](#setSource-com.aspose.zip.TarArchive-) | Sets the content to be compressed within the archive. |
| [setSource(File file)](#setSource-java.io.File-) | Sets the content to be compressed within the archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Sets the content to be compressed within the archive. |
| [setSource(String path)](#setSource-java.lang.String-) | Sets the content to be compressed within the archive. |
### GzipArchive() {#GzipArchive--}
```
public GzipArchive()
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for compressing.

The following example shows how to compress a file.

```

     try (GzipArchive archive = new GzipArchive())
     {
         archive.setSource("data.bin");
         archive.save("archive.gz");
     }
 
```



### GzipArchive(InputStream sourceStream) {#GzipArchive-java.io.InputStream-}
```
public GzipArchive(InputStream sourceStream)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### GzipArchive(InputStream sourceStream, boolean parseHeader) {#GzipArchive-java.io.InputStream-boolean-}
```
public GzipArchive(InputStream sourceStream, boolean parseHeader)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `ByteArrayOutputStream`

```

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive(Files.newInputStream(java.nio.file.Paths.get("archive.gz")))) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### GzipArchive(InputStream sourceStream, GzipLoadOptions options) {#GzipArchive-java.io.InputStream-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(InputStream sourceStream, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from a stream and extract it to a `MemoryStream`

```

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive(new FileInputStream("archive.gz"), options)) {
         archive.extract(ms);
     } catch (IOException ex) {
     }
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path, GzipLoadOptions options) {#GzipArchive-java.lang.String-com.aspose.zip.GzipLoadOptions-}
```
public GzipArchive(String path, GzipLoadOptions options)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class prepared for decompressing.

Open an archive from file by path and extract it to a `MemoryStream`

```

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     GzipLoadOptions options = new GzipLoadOptions();
     try (GzipArchive archive = new GzipArchive("archive.gz", options)) {
         archive.extract(ms);
     }
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| options | [GzipLoadOptions](../../com.aspose.zip/gziploadoptions) | Options to load the archive with. |

### GzipArchive(String path) {#GzipArchive-java.lang.String-}
```
public GzipArchive(String path)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |

### GzipArchive(String path, boolean parseHeader) {#GzipArchive-java.lang.String-boolean-}
```
public GzipArchive(String path, boolean parseHeader)
```


Initializes a new instance of the [GzipArchive](../../com.aspose.zip/gziparchive) class.

Open an archive from file by path and extract it to a `MemoryStream`

```

     ByteArrayOutputStream ms = new ByteArrayOutputStream();
     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         byte[] b = new byte[8192];
         int bytesRead;
         InputStream archiveStream = archive.open();
         while (0 < (bytesRead = archiveStream.read(b, 0, b.length))) {
             ms.write(b, 0, bytesRead);
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

This constructor does not decompress. See [open()](../../com.aspose.zip/gziparchive\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to the archive file. |
| parseHeader | boolean | Whether to parse stream header to figure out properties, including name. Makes sense for seekable stream only. |

### close() {#close--}
```
public void close()
```




### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the archive to the stream provided.

```

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         archive.extract(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | Destination stream. Must be writable. |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

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
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the gzip archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the gzip archive.
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Gets the archive format.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - the archive format
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets size of an original file.

During decompression, this property may contain incorrect size. If the uncompressed file size exceeds 4GB, this property will give a wrong value due to the 32-bit limit in header.

**Returns:**
java.lang.Long - size of an original file
### getName() {#getName--}
```
public final String getName()
```


The name of the original file.

**Returns:**
java.lang.String - the name of the original file
### getUncompressedSize() {#getUncompressedSize--}
```
public final long getUncompressedSize()
```


Gets size of an original file.

During decompression, this property may contain incorrect size. If the uncompressed file size exceeds 4GB, this property will give a wrong value due to the 32-bit limit in header.

**Returns:**
long - size of an original file.
### open() {#open--}
```
public final InputStream open()
```


Opens the archive for extraction and provides a stream with archive content.

Extracts the archive and copies extracted content to file stream.

```

     try (GzipArchive archive = new GzipArchive("archive.gz")) {
         try (FileOutputStream extracted = new FileOutputStream("data.bin")) {
             InputStream unpacked = archive.open();
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 < (bytesRead = unpacked.read(b, 0, b.length))) {
                 extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
         System.out.println(ex);
     }
 
```

Read from the stream to get the original content of a file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the archive.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

Writes compressed data to http response stream.

```

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save(httpResponseStream);
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream.

`outputStream` must be writable. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to the destination file provided.

```

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### setSource(TarArchive tarArchive) {#setSource-com.aspose.zip.TarArchive-}
```
public final void setSource(TarArchive tarArchive)
```


Sets the content to be compressed within the archive.

```

     try (TarArchive tarArchive = new TarArchive()) {
         tarArchive.createEntry("first.bin", "data1.bin");
         tarArchive.createEntry("second.bin", "data2.bin");
         try (GzipArchive gzippedArchive = new GzipArchive()) {
             gzippedArchive.setSource(tarArchive);
             gzippedArchive.save("archive.tar.gz");
         }
     }
 
```

Use this method to compose joint tar.gz archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tarArchive | [TarArchive](../../com.aspose.zip/tararchive) | Tar archive to be compressed. |

### setSource(File file) {#setSource-java.io.File-}
```
public final void setSource(File file)
```


Sets the content to be compressed within the archive.

```

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | The reference to a file to be compressed. |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | The input stream for the archive. |

### setSource(String path) {#setSource-java.lang.String-}
```
public final void setSource(String path)
```


Sets the content to be compressed within the archive.

Open an archive from file by path and extract it to a `MemoryStream`

```

     try (GzipArchive archive = new GzipArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.gz");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | Path to file to be compressed. |

