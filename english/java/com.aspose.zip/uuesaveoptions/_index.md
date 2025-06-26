---
title: UueSaveOptions
second_title: Aspose.ZIP for Java API Reference
description: Options for saving an uuencoded file.
type: docs
weight: 103
url: /java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Options for saving an uuencoded file.
## Constructors

| Constructor | Description |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Initializes the options with user provided file name and new line. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Initializes the options with user provided file name and the default new line. |
## Methods

| Method | Description |
| --- | --- |
| [getFileName()](#getFileName--) | Gets the file name to be used when recreating the decoded data. |
| [getNewLine()](#getNewLine--) | Gets the character terminating each line, usually "\\n" or "\\r\\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Gets the file's Unix file permissions. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Sets the file's Unix file permissions. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Initializes the options with user provided file name and new line.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the file name to be used when recreating the decoded data |
| newLine | java.lang.String | the character terminating each line |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Initializes the options with user provided file name and the default new line.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the file name to be used when recreating the decoded data |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Gets the file name to be used when recreating the decoded data.

**Returns:**
java.lang.String - the file name to be used when recreating the decoded data
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Gets the character terminating each line, usually "\\n" or "\\r\\n".

**Returns:**
java.lang.String - the character terminating each line, usually "\\n" or "\\r\\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Gets the file's Unix file permissions.

Default is 644.

**Returns:**
java.lang.String - the file's Unix file permissions
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Sets the file's Unix file permissions.

Default is 644.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | the file's Unix file permissions |

