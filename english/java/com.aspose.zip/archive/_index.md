---
title: Archive
second_title: Aspose.ZIP for Java API Reference
description: This class represents zip archive file.
type: docs
weight: 11
url: /java/com.aspose.zip/archive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IDisposable, [com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class Archive implements System.IDisposable, IArchive, AutoCloseable
```

This class represents zip archive file. Use it to compose, extract, or update zip archives.
## Constructors

| Constructor | Description |
| --- | --- |
| [Archive()](#Archive--) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries. |
| [Archive(ArchiveEntrySettings newEntrySettings)](#Archive-com.aspose.zip.ArchiveEntrySettings-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries. |
| [Archive(InputStream sourceStream)](#Archive-java.io.InputStream-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive. |
| [Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive. |
| [Archive(String path)](#Archive-java.lang.String-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive. |
| [Archive(String path, ArchiveLoadOptions loadOptions)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive. |
| [Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)](#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-) | Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Adds to the archive all files and directories recursively in the directory given. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Adds to the archive all files and directories recursively in the directory given. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Adds to the archive all files and directories recursively in the directory given. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Adds to the archive all files and directories recursively in the directory given. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Create single entry within the archive. |
| [createEntry(String name, File file, boolean openImmediately)](#createEntry-java.lang.String-java.io.File-boolean-) | Create single entry within the archive. |
| [createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-) | Create single entry within the archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Create single entry within the archive. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-) | Create single entry within the archive. |
| [createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)](#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-) | Create single entry within the archive. |
| [createEntry(String name, String path)](#createEntry-java.lang.String-java.lang.String-) | Create single entry within the archive. |
| [createEntry(String name, String path, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Create single entry within the archive. |
| [createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)](#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-) | Create single entry within the archive. |
| [deleteEntry(ArchiveEntry entry)](#deleteEntry-com.aspose.zip.ArchiveEntry-) | Removes the first occurrence of a specific entry from the entries list. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Removes the entry from the entries list by index. |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts all the files in the archive to the directory provided. |
| [getEntries()](#getEntries--) | Gets entries of [ArchiveEntry](../../com.aspose.zip/archiveentry) type constituting the archive. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive. |
| [getNewEntrySettings()](#getNewEntrySettings--) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. |
| [save(OutputStream outputStream)](#save-java.io.OutputStream-) | Saves archive to the stream provided. |
| [save(OutputStream outputStream, ArchiveSaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-) | Saves archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves archive to destination file provided. |
| [save(String destinationFileName, ArchiveSaveOptions saveOptions)](#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-) | Saves archive to destination file provided. |
| [saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)](#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-) | Saves multi-volume archive to destination directory provided. |
### Archive() {#Archive--}
```
public Archive()
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

### Archive(ArchiveEntrySettings newEntrySettings) {#Archive-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class with optional settings for its entries.


The following example shows how to compress a single file with default settings.

```

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, most common Deflate compression without encryption would be used. |

### Archive(InputStream sourceStream) {#Archive-java.io.InputStream-}
```
public Archive(InputStream sourceStream)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive.


The following example extract an encrypted archive, then decompress first entry to a  ByteArrayOutputStream .

```

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 &lt; (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive.


The following example extract an encrypted archive, then decompress first entry to a  ByteArrayOutputStream .

```

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 &lt; (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.io.InputStream-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(InputStream sourceStream, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive.


The following example extract an encrypted archive, then decompress first entry to a  ByteArrayOutputStream .

```

     try (FileInputStream fs = new FileInputStream("encrypted.zip")) {
         ByteArrayOutputStream extracted = new ByteArrayOutputStream();
         ArchiveLoadOptions options = new ArchiveLoadOptions();
         options.setDecryptionPassword("p@s$");
         try (Archive archive = new Archive(fs, options)) {
             try (InputStream decompressed = archive.getEntries().get(0).open()) {
                 byte[] b = new byte[8192];
                 int bytesRead;
                 while (0 &lt; (bytesRead = decompressed.read(b, 0, b.length)))
                     extracted.write(b, 0, bytesRead);
             }
         }
     } catch (IOException ex) {
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | The source of the archive. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, most common Deflate compression without encryption would be used. |

### Archive(String path) {#Archive-java.lang.String-}
```
public Archive(String path)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive.


The following example extract an encrypted archive, then decompress first entry to a  ByteArrayOutputStream .

```

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 &lt; (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |

### Archive(String path, ArchiveLoadOptions loadOptions) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-}
```
public Archive(String path, ArchiveLoadOptions loadOptions)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive.


The following example extract an encrypted archive, then decompress first entry to a  ByteArrayOutputStream .

```

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 &lt; (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |

### Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings) {#Archive-java.lang.String-com.aspose.zip.ArchiveLoadOptions-com.aspose.zip.ArchiveEntrySettings-}
```
public Archive(String path, ArchiveLoadOptions loadOptions, ArchiveEntrySettings newEntrySettings)
```


Initializes a new instance of the [Archive](../../com.aspose.zip/archive) class and composes entries list can be extracted from the archive.


The following example extract an encrypted archive, then decompress first entry to a  ByteArrayOutputStream .

```

     ByteArrayOutputStream extracted = new ByteArrayOutputStream();
     ArchiveLoadOptions options = new ArchiveLoadOptions();
     options.setDecryptionPassword("p@s$");
     try (Archive archive = new Archive("encrypted.zip", options)) {
         try (InputStream decompressed = archive.getEntries().get(0).open()) {
             byte[] b = new byte[8192];
             int bytesRead;
             while (0 &lt; (bytesRead = decompressed.read(b, 0, b.length)))
                 extracted.write(b, 0, bytesRead);
         } catch (IOException ex) {
         }
     }
 
```

This constructor does not decompress any entry. See [ArchiveEntry.open()](../../com.aspose.zip/archiveentry\#open--) method for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The fully qualified or the relative path to the archive file. |
| loadOptions | [ArchiveLoadOptions](../../com.aspose.zip/archiveloadoptions) | Options to load existing archive with. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items. If not specified, most common Deflate compression without encryption would be used. |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final Archive createEntries(File directory)
```


Adds to the archive all files and directories recursively in the directory given.

```

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final Archive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

    try (Archive archive = new Archive()) {
        java.io.File folder = new java.io.File("C:\\folder");
        archive.createEntries(folder);
        archive.save("folder.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory itself or not. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final Archive createEntries(String sourceDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final Archive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all files and directories recursively in the directory given.

```

    try (Archive archive = new Archive()) {
        archive.createEntries("C:\\folder");
        archive.save("folder.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | Directory to compress. |
| includeRootDirectory | boolean | Indicates whether to include the root directory itself or not. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with entries composed.
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final ArchiveEntry createEntry(String name, File file)
```


Create single entry within the archive.


Compose archive with entries encrypted with different encryption methods and passwords each.

```

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

The entry name is solely set within  name  parameter. The file name provided in  fileInfo  parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately)
```


Create single entry within the archive.


Compose archive with entries encrypted with different encryption methods and passwords each.

```

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

The entry name is solely set within  name  parameter. The file name provided in  fileInfo  parameter does not affect the entry name.

If the file is opened immediately with  openImmediately  parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True if open the file immediately, otherwise open the file on archive saving. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.File-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, File file, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Create single entry within the archive.


Compose archive with entries encrypted with different encryption methods and passwords each.

```

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        java.io.File fi1 = new java.io.File("data1.bin");
        java.io.File fi2 = new java.io.File("data2.bin");
        java.io.File fi3 = new java.io.File("data3.bin");
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", fi1, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")));
            archive.createEntry("entry2.bin", fi2, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass2", EncryptionMethod.AES128)));
            archive.createEntry("entry3.bin", fi3, false, new ArchiveEntrySettings(new DeflateCompressionSettings(), new AesEncryptionSettings("pass3", EncryptionMethod.AES256)));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

The entry name is solely set within  name  parameter. The file name provided in  fileInfo  parameter does not affect the entry name.

If the file is opened immediately with  openImmediately  parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| file | java.io.File | The metadata of file to be compressed. |
| openImmediately | boolean | True if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final ArchiveEntry createEntry(String name, InputStream source)
```


Create single entry within the archive.

```

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings)
```


Create single entry within the archive.

```

     try (Archive archive = new Archive(new ArchiveEntrySettings(null, new AesEncryptionSettings("p@s$", EncryptionMethod.AES256)))) {
         archive.createEntry("data.bin", new ByteArrayInputStream(new byte[] {
                 0x00,
                 (byte) 0xFF
         }));
         archive.save("archive.zip");
     }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file) {#createEntry-java.lang.String-java.io.InputStream-com.aspose.zip.ArchiveEntrySettings-java.io.File-}
```
public final ArchiveEntry createEntry(String name, InputStream source, ArchiveEntrySettings newEntrySettings, File file)
```


Create single entry within the archive.


Compose archive with encrypted entry.

```

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry1.bin", new ByteArrayInputStream(new byte[] {
                    0x00,
                    (byte) 0xFF
            }), new ArchiveEntrySettings(new DeflateCompressionSettings(), new TraditionalEncryptionSettings("pass1")), new java.io.File("data1.bin"));
            archive.save(zipFile);
        }
    } catch (IOException ignored) {
    }
 
```

The entry name is solely set within  name  parameter. The file name provided in  fileInfo  parameter does not affect the entry name.

 fileInfo  can refer to DirectoryInfo if the entry is directory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| source | java.io.InputStream | The input stream for the entry. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |
| file | java.io.File | The metadata of file or folder to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path) {#createEntry-java.lang.String-java.lang.String-}
```
public final ArchiveEntry createEntry(String name, String path)
```


Create single entry within the archive.

```

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

The entry name is solely set within  name  parameter. The file name provided in  path  parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately)
```


Create single entry within the archive.

```

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

The entry name is solely set within  name  parameter. The file name provided in  path  parameter does not affect the entry name.

If the file is opened immediately with  openImmediately  parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True if open the file immediately, otherwise open the file on archive saving. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings) {#createEntry-java.lang.String-java.lang.String-boolean-com.aspose.zip.ArchiveEntrySettings-}
```
public final ArchiveEntry createEntry(String name, String path, boolean openImmediately, ArchiveEntrySettings newEntrySettings)
```


Create single entry within the archive.

```

     try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
         try (Archive archive = new Archive()) {
             archive.createEntry("data.bin", "file.dat");
             archive.save(zipFile);
         }
     } catch (IOException ex) {
     }
 
```

The entry name is solely set within  name  parameter. The file name provided in  path  parameter does not affect the entry name.

If the file is opened immediately with  openImmediately  parameter it becomes blocked until archive is saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The name of the entry. |
| path | java.lang.String | The fully qualified name of the new file, or the relative file name to be compressed. |
| openImmediately | boolean | True if open the file immediately, otherwise open the file on archive saving. |
| newEntrySettings | [ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) | Compression and encryption settings used for added [ArchiveEntry](../../com.aspose.zip/archiveentry) item. |

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - Zip entry instance.
### deleteEntry(ArchiveEntry entry) {#deleteEntry-com.aspose.zip.ArchiveEntry-}
```
public final Archive deleteEntry(ArchiveEntry entry)
```


Removes the first occurrence of a specific entry from the entries list.


Here is how you can remove all entries except the last one:

```

    try (Archive archive = new Archive("archive.zip")) {
        while (archive.getEntries().size() &gt; 1)
            archive.deleteEntry(archive.getEntries().get(0));
        archive.save("last_entry.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | The entry to remove from the entries list. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final Archive deleteEntry(int entryIndex)
```


Removes the entry from the entries list by index.

```

    try (Archive archive = new Archive("two_files.zip")) {
        archive.deleteEntry(0);
        archive.save("single_file.zip");
    }
 
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | The zero-based index of the entry to remove. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - The archive with the entry deleted.
### dispose() {#dispose--}
```
public final void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts all the files in the archive to the directory provided.

```

    try (Archive archive = new Archive("archive.zip")) {
        archive.extractToDirectory("C:\\extracted");
    }
 
```

If the directory does not exist, it will be created.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory to place the extracted files in. |

### getEntries() {#getEntries--}
```
public final List<ArchiveEntry> getEntries()
```


Gets entries of [ArchiveEntry](../../com.aspose.zip/archiveentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.ArchiveEntry&gt; - entries of [ArchiveEntry](../../com.aspose.zip/archiveentry) type constituting the archive.
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the archive.
### getNewEntrySettings() {#getNewEntrySettings--}
```
public final ArchiveEntrySettings getNewEntrySettings()
```


Compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items.

**Returns:**
[ArchiveEntrySettings](../../com.aspose.zip/archiveentrysettings) - compression and encryption settings used for newly added [ArchiveEntry](../../com.aspose.zip/archiveentry) items.
### save(OutputStream outputStream) {#save-java.io.OutputStream-}
```
public final void save(OutputStream outputStream)
```


Saves archive to the stream provided.

```

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

 outputStream  must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |

### save(OutputStream outputStream, ArchiveSaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(OutputStream outputStream, ArchiveSaveOptions saveOptions)
```


Saves archive to the stream provided.

```

    try (FileOutputStream zipFile = new FileOutputStream("archive.zip")) {
        try (Archive archive = new Archive()) {
            archive.createEntry("entry.bin", "data.bin");
            archive.save(zipFile);
        }
    } catch (IOException ex) {
    }
 
```

 outputStream  must be writable.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| outputStream | java.io.OutputStream | Destination stream. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Options for archive saving. |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to destination file provided.

```

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |

### save(String destinationFileName, ArchiveSaveOptions saveOptions) {#save-java.lang.String-com.aspose.zip.ArchiveSaveOptions-}
```
public final void save(String destinationFileName, ArchiveSaveOptions saveOptions)
```


Saves archive to destination file provided.

```

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        ArchiveSaveOptions options = new ArchiveSaveOptions();
        options.setEncoding(StandardCharsets.US_ASCII);
        archive.save("archive.zip", options);
    }
 
```

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | The path of the archive to be created. If the specified file name points to an existing file, it will be overwritten. |
| saveOptions | [ArchiveSaveOptions](../../com.aspose.zip/archivesaveoptions) | Options for archive saving. |

### saveSplit(String destinationDirectory, SplitArchiveSaveOptions options) {#saveSplit-java.lang.String-com.aspose.zip.SplitArchiveSaveOptions-}
```
public final void saveSplit(String destinationDirectory, SplitArchiveSaveOptions options)
```


Saves multi-volume archive to destination directory provided.

```

    try (Archive archive = new Archive()) {
        archive.createEntry("entry.bin", "data.bin");
        archive.saveSplit( "C:\\Folder", new SplitArchiveSaveOptions("volume", 65536));
    }
 
```

This method compose several (n) files filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Can not make existing archive multi-volume.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | The path to the directory where archive segments to be created. |
| options | [SplitArchiveSaveOptions](../../com.aspose.zip/splitarchivesaveoptions) | Options for archive saving, including file name. |

