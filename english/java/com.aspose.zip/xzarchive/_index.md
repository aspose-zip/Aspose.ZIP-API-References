---
title: XzArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents xz archive file.
type: docs
weight: 84
url: /java/com.aspose.zip/xzarchive/
---

**Inheritance:**
java.lang.Object, com.aspose.zip.ILicenseStateProvider

**All Implemented Interfaces:**
[com.aspose.zip.IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry), com.aspose.ms.System.IDisposable, [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class XzArchive extends ILicenseStateProvider implements IArchiveFileEntry, System.IDisposable, IArchive, AutoCloseable
```

This class represents xz archive file. Use it to compose and extract xz archives.
## Constructors

| Constructor | Description |
| --- | --- |
| [XzArchive()](#XzArchive--) | Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class and composes the archive in xz format. |
| [XzArchive(XzArchiveSettings settings)](#XzArchive-com.aspose.zip.XzArchiveSettings-) | Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class and composes the archive in xz format. |
| [XzArchive(InputStream source)](#XzArchive-java.io.InputStream-) | Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class prepared for decompressing. |
| [XzArchive(String path)](#XzArchive-java.lang.String-) | Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class prepared for decompressing. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [extract(File file)](#extract-java.io.File-) | Extracts xz archive to a file. |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts xz archive to a stream. |
| [extract(String path)](#extract-java.lang.String-) | Extracts xz archive to a file by path. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts content of the archive to the directory provided. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive. |
| [getLength()](#getLength--) | Gets the length of the entry in bytes. |
| [getName()](#getName--) | Gets the name of the entry within archive. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves xz archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves xz archive to destination file provided. |
| [setSource(File file)](#setSource-java.io.File-) | Sets the content to be compressed within the archive. |
| [setSource(InputStream source)](#setSource-java.io.InputStream-) | Sets the content to be compressed within the archive. |
| [setSource(String sourcePath)](#setSource-java.lang.String-) | Sets the content to be compressed within the archive. |
### XzArchive() {#XzArchive--}
```
public XzArchive()
```


Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class and composes the archive in xz format.

### XzArchive(XzArchiveSettings settings) {#XzArchive-com.aspose.zip.XzArchiveSettings-}
```
public XzArchive(XzArchiveSettings settings)
```


Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class and composes the archive in xz format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) | set of setting particular xz archive: dictionary size, block size, check type |

### XzArchive(InputStream source) {#XzArchive-java.io.InputStream-}
```
public XzArchive(InputStream source)
```


Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | java.io.InputStream | the source of the archive |

### XzArchive(String path) {#XzArchive-java.lang.String-}
```
public XzArchive(String path)
```


Initializes a new instance of the [XzArchive](../../com.aspose.zip/xzarchive) class prepared for decompressing.

This constructor does not decompress. See [extract(java.io.OutputStream)](../../com.aspose.zip/xzarchive\#extract-java.io.OutputStream-) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to the source of the archive |

### close() {#close--}
```
public void close()
```




### dispose() {#dispose--}
```
public final void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### extract(File file) {#extract-java.io.File-}
```
public final void extract(File file)
```


Extracts xz archive to a file.

```

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (XzArchive archive = new XzArchive(xzFile)) {
             archive.extract(new File("extracted.bin"));
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file for storing decompressed data |

### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts xz archive to a stream.

```

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (FileOutputStream extractedFile = new FileOutputStream("extractedFileName")) {
             try (XzArchive archive = new XzArchive(xzFile)) {
                 archive.extract(extractedFile);
             }
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destination | java.io.OutputStream | stream for storing decompressed data |

### extract(String path) {#extract-java.lang.String-}
```
public final File extract(String path)
```


Extracts xz archive to a file by path.

```

     try (FileInputStream xzFile = new FileInputStream("sourceFileName")) {
         try (XzArchive archive = new XzArchive(xzFile)) {
             archive.extract("extracted.bin");
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | path to file which will store decompressed data |

**Returns:**
java.io.File - java.io.File instance containing extracted data
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts content of the archive to the directory provided.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created. |

### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the xz archive
### getLength() {#getLength--}
```
public final Long getLength()
```


Gets the length of the entry in bytes.

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


Saves xz archive to the stream provided.

```

     try (FileOutputStream xzFile = new FileOutputStream("archive.xz")) {
         try (XzArchive archive = new XzArchive()) {
             archive.setSource("data.bin");
             archive.save(xzFile);
         }
     } catch (IOException ex) {
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


Saves xz archive to destination file provided.

```

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("result.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new File("data.bin"));
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.io.File | file which will be opened as input stream |

### setSource(InputStream source) {#setSource-java.io.InputStream-}
```
public final void setSource(InputStream source)
```


Sets the content to be compressed within the archive.

```

     try (XzArchive archive = new XzArchive()) {
         archive.setSource(new ByteArrayInputStream(new byte[] { 0x00, (byte) 0xFF }));
         archive.save("archive.xz");
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

     try (XzArchive archive = new XzArchive()) {
         archive.setSource("data.bin");
         archive.save("archive.xz");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourcePath | java.lang.String | path to file which will be opened as input stream |

