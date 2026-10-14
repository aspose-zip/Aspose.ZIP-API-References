---
title: "ArchiveInstanceInfo"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Stellt Informationen über die Archivinstanz dar."
type: docs
weight: 34
url: /de/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Stellt Informationen über die Archivinstanz dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Gibt einen Wert zurück, der angibt, ob die Namen der Einträge (Dateien) des Archivs verschlüsselt sind. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Gibt Informationen zum Archivformat zurück. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Gibt Informationen zum Archivformat zurück. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Gibt Informationen zur Archivinstanz zurück. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Gibt Informationen zur Archivinstanz zurück. |
| [getFormatInfo()](#getFormatInfo--) | Gibt die Informationen zum Archivformat zurück. |
| [isContentEncrypted()](#isContentEncrypted--) | Gibt einen Wert zurück, der angibt, ob der Inhalt des Archivs verschlüsselt ist. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Gibt einen Wert zurück, der angibt, ob die Namen der Einträge (Dateien) des Archivs verschlüsselt sind.

**Returns:**
boolean - ein Wert, der angibt, ob die Namen der Einträge (Dateien) des Archivs verschlüsselt sind.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Gibt Informationen zum Archivformat zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Der Stream der Archivdatei. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Gibt Informationen zum Archivformat zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname der Archivdatei. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Gibt Informationen zur Archivinstanz zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stream | java.io.InputStream | Der Stream der Archivdatei. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Gibt Informationen zur Archivinstanz zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname der Archivdatei. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Gibt die Informationen zum Archivformat zurück.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Gibt einen Wert zurück, der angibt, ob der Inhalt des Archivs verschlüsselt ist.

**Returns:**
boolean - ein Wert, der angibt, ob der Inhalt des Archivs verschlüsselt ist.
