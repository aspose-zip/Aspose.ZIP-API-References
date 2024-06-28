---
title: WimArchive
second_title: Aspose.ZIP for Java API Reference
description: This class represents wim archive file.
type: docs
weight: 71
url: /java/com.aspose.zip/wimarchive/
---

**Inheritance:**
java.lang.Object, com.aspose.zip.ILicenseStateProvider

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class WimArchive extends ILicenseStateProvider implements IArchive, AutoCloseable
```

This class represents wim archive file.
## Constructors

| Constructor | Description |
| --- | --- |
| [WimArchive(InputStream sourceStream)](#WimArchive-java.io.InputStream-) | Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes entries list can be extracted from the archive. |
| [WimArchive(String path)](#WimArchive-java.lang.String-) | Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes entries list can be extracted from the archive. |
## Methods

| Method | Description |
| --- | --- |
| [close()](#close--) | \{@inheritDoc\} |
| [dispose()](#dispose--) | Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Extracts the archive to the file by path. |
| [getBootImageIndex()](#getBootImageIndex--) | Gets the (zero-based) index of the bootable image. |
| [getFileEntries()](#getFileEntries--) | Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the wim archive. |
| [getFileFormatVersion()](#getFileFormatVersion--) | Gets the version of the file format. |
| [getGuid()](#getGuid--) | Gets the identifying UUID for the archive. |
| [getManifest()](#getManifest--) | Gets the embedded manifest describing the file and the contained images. |
### WimArchive(InputStream sourceStream) {#WimArchive-java.io.InputStream-}
```
public WimArchive(InputStream sourceStream)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes entries list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

     try (WimArchive archive = new WimArchive(new FileInputStream("archive.wim"))) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     } catch (IOException ex) {
     }
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceStream | java.io.InputStream | the source of the archive |

### WimArchive(String path) {#WimArchive-java.lang.String-}
```
public WimArchive(String path)
```


Initializes a new instance of the [WimArchive](../../com.aspose.zip/wimarchive) class and composes entries list can be extracted from the archive.

The following example shows how to extract all of the entries to a directory.

```

     try (WimArchive archive = new WimArchive("archive.wim")) {
         archive.getImages().get_Item(0).extractToDirectory("C:\\extracted");
     }
 
```

This constructor does not unpack any entry. See [WimFileEntry.open()](../../com.aspose.zip/wimfileentry\#open--) method for unpacking.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path to the archive file |

### close() {#close--}
```
public void close()
```




### dispose() {#dispose--}
```
public final void dispose()
```


Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Extracts the archive to the file by path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in |

### getBootImageIndex() {#getBootImageIndex--}
```
public final int getBootImageIndex()
```


Gets the (zero-based) index of the bootable image.

**Returns:**
int - the (zero-based) index of the bootable image
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Gets entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the wim archive.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - entries of [IArchiveFileEntry](../../com.aspose.zip/iarchivefileentry) type constituting the wim archive
### getFileFormatVersion() {#getFileFormatVersion--}
```
public final int getFileFormatVersion()
```


Gets the version of the file format.

**Returns:**
int - the version of the file format
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


Gets the identifying UUID for the archive.

**Returns:**
java.util.UUID - the identifying UUID for the archive
### getManifest() {#getManifest--}
```
public final String getManifest()
```


Gets the embedded manifest describing the file and the contained images.

**Returns:**
java.lang.String - the embedded manifest describing the file and the contained images
