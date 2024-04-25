---
title: TarEntry
second_title: Aspose.ZIP for Java API Reference
description: Represents single file within tar archive.
type: docs
weight: 61
url: /java/com.aspose.zip/tarentry/
---

**Inheritance:**
java.lang.Object
```
public class TarEntry
```

Represents single file within tar archive.
## Methods

| Method | Description |
| --- | --- |
| [extract(OutputStream destination)](#extract-java.io.OutputStream-) | Extracts the entry to the stream provided. |
| [extract(String path)](#extract-java.lang.String-) | Extracts the entry to the filesystem by the path provided. |
| [getLength()](#getLength--) | Get length of entry in bytes. |
| [getName()](#getName--) | Gets name of the entry within archive. |
| [isDirectory()](#isDirectory--) | Gets a value indicating whether the entry represents directory. |
| [open()](#open--) | Opens the entry for extraction and provides a stream with entry content. |
| [setName(String value)](#setName-java.lang.String-) | Sets name of the entry within archive. |
### extract(OutputStream destination) {#extract-java.io.OutputStream-}
```
public final void extract(OutputStream destination)
```


Extracts the entry to the stream provided.

Extract an entry of tar archive.

```

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract(httpResponseStream);
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


Extracts the entry to the filesystem by the path provided.

```

     try (TarArchive archive = new TarArchive("archive.tar")) {
         archive.getEntries().get_Item(0).extract("data.bin");
     }
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to destination file. If the file already exists, it will be overwritten. |

**Returns:**
java.io.File - The file info of composed file.
### getLength() {#getLength--}
```
public final long getLength()
```


Get length of entry in bytes.

**Returns:**
long - length of entry in bytes.
### getName() {#getName--}
```
public final String getName()
```


Gets name of the entry within archive.

**Returns:**
java.lang.String - name of the entry within archive.
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Gets a value indicating whether the entry represents directory.

**Returns:**
boolean - a value indicating whether the entry represents directory.
### open() {#open--}
```
public final InputStream open()
```


Opens the entry for extraction and provides a stream with entry content.


Usage:

```

     InputStream decompressed = entry.open();
     byte[] buffer = new byte[8192];
     int bytesRead;
     while (0 < (bytesRead = decompressed.read(buffer, 0, buffer.length))) {
         fileStream.write(buffer, 0, bytesRead);
     }
 
```

Read from the stream to get original content of file. See examples section.

**Returns:**
java.io.InputStream - The stream that represents the contents of the entry.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets name of the entry within archive.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | name of the entry within archive. |

