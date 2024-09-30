---
title: SharArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents shar archive file.
type: docs
weight: 77
url: /java/com.aspose.zip/shararchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class SharArchive implements AutoCloseable
```

This class represents shar archive file.
## Constructors

| Constructor | Description |
| --- | --- |
| [SharArchive()](#SharArchive--) | Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class. |
| [SharArchive(String path)](#SharArchive-java.lang.String-) | Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [createEntries(File directory)](#createEntries-java.io.File-) | Adds to the archive all the files and directories recursively in the directory given. |
| [createEntries(File directory, boolean includeRootDirectory)](#createEntries-java.io.File-boolean-) | Adds to the archive all the files and directories recursively in the directory given. |
| [createEntries(String sourceDirectory)](#createEntries-java.lang.String-) | Adds to the archive all the files and directories recursively in the directory given. |
| [createEntries(String sourceDirectory, boolean includeRootDirectory)](#createEntries-java.lang.String-boolean-) | Adds to the archive all the files and directories recursively in the directory given. |
| [createEntry(String name, File file)](#createEntry-java.lang.String-java.io.File-) | Create single entry within the archive. |
| [createEntry(String name, File file, boolean includeRootDirectory)](#createEntry-java.lang.String-java.io.File-boolean-) | Create single entry within the archive. |
| [createEntry(String name, InputStream source)](#createEntry-java.lang.String-java.io.InputStream-) | Create single entry within the archive. |
| [createEntry(String name, String sourcePath)](#createEntry-java.lang.String-java.lang.String-) | Create single entry within the archive. |
| [createEntry(String name, String sourcePath, boolean openImmediately)](#createEntry-java.lang.String-java.lang.String-boolean-) | Create single entry within the archive. |
| [deleteEntry(SharEntry entry)](#deleteEntry-com.aspose.zip.SharEntry-) | Removes the first occurrence of a specific entry from the entries list. |
| [deleteEntry(int entryIndex)](#deleteEntry-int-) | Removes the entry from the entries list by index. |
| [getEntries()](#getEntries--) | Gets entries of [SharEntry](../../com.aspose.zip/sharentry) type constituting the archive. |
| [save(OutputStream output)](#save-java.io.OutputStream-) | Saves archive to the stream provided. |
| [save(String destinationFileName)](#save-java.lang.String-) | Saves archive to destination file provided. |
### SharArchive() {#SharArchive--}
```
public SharArchive()
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class.

The following example shows how to compress a file.

```

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```



### SharArchive(String path) {#SharArchive-java.lang.String-}
```
public SharArchive(String path)
```


Initializes a new instance of the [SharArchive](../../com.aspose.zip/shararchive) class prepared for decompressing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the source of the archive |

### close() {#close--}
```
public void close()
```




### createEntries(File directory) {#createEntries-java.io.File-}
```
public final SharArchive createEntries(File directory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(File directory, boolean includeRootDirectory) {#createEntries-java.io.File-boolean-}
```
public final SharArchive createEntries(File directory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries(new java.io.File("C:\\folder"), false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| directory | java.io.File | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory) {#createEntries-java.lang.String-}
```
public final SharArchive createEntries(String sourceDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntries(String sourceDirectory, boolean includeRootDirectory) {#createEntries-java.lang.String-boolean-}
```
public final SharArchive createEntries(String sourceDirectory, boolean includeRootDirectory)
```


Adds to the archive all the files and directories recursively in the directory given.

```

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntries("C:\\folder", false);
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceDirectory | java.lang.String | the directory to compress |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### createEntry(String name, File file) {#createEntry-java.lang.String-java.io.File-}
```
public final SharEntry createEntry(String name, File file)
```


Create single entry within the archive.

```

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, File file, boolean includeRootDirectory) {#createEntry-java.lang.String-java.io.File-boolean-}
```
public final SharEntry createEntry(String name, File file, boolean includeRootDirectory)
```


Create single entry within the archive.

```

     java.io.File file = new java.io.File("data.bin");
     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("test.bin", file);
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| file | java.io.File | the metadata of file or folder to be compressed |
| includeRootDirectory | boolean | indicates whether to include the root directory itself or not |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, InputStream source) {#createEntry-java.lang.String-java.io.InputStream-}
```
public final SharEntry createEntry(String name, InputStream source)
```


Create single entry within the archive.

```

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("data.bin", new FileInputStream("data.bin"));
         archive.save("archive.shar");
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| source | java.io.InputStream | the input stream for the entry |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath) {#createEntry-java.lang.String-java.lang.String-}
```
public final SharEntry createEntry(String name, String sourcePath)
```


Create single entry within the archive.

```

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to the file to be compressed |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### createEntry(String name, String sourcePath, boolean openImmediately) {#createEntry-java.lang.String-java.lang.String-boolean-}
```
public final SharEntry createEntry(String name, String sourcePath, boolean openImmediately)
```


Create single entry within the archive.

```

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("first.bin", "data.bin");
         archive.save("archive.shar");
     }
 
```

The entry name is solely set within `name` parameter. The file name provided in `sourcePath` parameter does not affect the entry name.

If the file is opened immediately with `openImmediately` parameter it becomes blocked until archive is disposed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | the name of the entry |
| sourcePath | java.lang.String | the path to file to be compressed |
| openImmediately | boolean | true if open the file immediately, otherwise open the file on archive saving |

**Returns:**
[SharEntry](../../com.aspose.zip/sharentry) - Shar entry instance
### deleteEntry(SharEntry entry) {#deleteEntry-com.aspose.zip.SharEntry-}
```
public final SharArchive deleteEntry(SharEntry entry)
```


Removes the first occurrence of a specific entry from the entries list.

Here is how you can remove all entries except the last one:

```

     try (SharArchive archive = new SharArchive("archive.shar")) {
         while (archive.getEntries().size() > 1)
             archive.deleteEntry(archive.getEntries().get(0));
         archive.save("outputSharFile.shar");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entry | [SharEntry](../../com.aspose.zip/sharentry) | the entry to remove from the entries list |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - Shar entry instance
### deleteEntry(int entryIndex) {#deleteEntry-int-}
```
public final SharArchive deleteEntry(int entryIndex)
```


Removes the entry from the entries list by index.

```

     try (SharArchive archive = new SharArchive("two_files.shar")) {
         archive.deleteEntry(0);
         archive.save("single_file.shar");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| entryIndex | int | the zero-based index of the entry to remove |

**Returns:**
[SharArchive](../../com.aspose.zip/shararchive) - the archive with the entry deleted
### getEntries() {#getEntries--}
```
public final List<SharEntry> getEntries()
```


Gets entries of [SharEntry](../../com.aspose.zip/sharentry) type constituting the archive.

**Returns:**
java.util.List&lt;com.aspose.zip.SharEntry&gt; - entries of [SharEntry](../../com.aspose.zip/sharentry) type constituting the archive
### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Saves archive to the stream provided.

```

     try (FileOutputStream sharFile = new FileOutputStream("archive.shar")) {
         try (SharArchive archive = new SharArchive()) {
             archive.createEntry("entry1", "data.bin");
             archive.save(sharFile);
         }
     } catch (IOException ex) {
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| output | java.io.OutputStream | the destination stream |

### save(String destinationFileName) {#save-java.lang.String-}
```
public final void save(String destinationFileName)
```


Saves archive to destination file provided.

```

     try (SharArchive archive = new SharArchive()) {
         archive.createEntry("entry1", "data.bin");
         archive.save("archive.shar");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationFileName | java.lang.String | the path of the archive to be created. If the specified file name points to an existing file, it will be overwritten.

It is possible to save an archive to the same path as it was loaded from. However, this is not recommended because this approach uses copying to temporary file |

