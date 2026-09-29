---
title: "ArchiveInstanceInfo"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rappresenta informazioni sull'istanza dell'archivio."
type: docs
weight: 34
url: /it/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Rappresenta informazioni sull'istanza dell'archivio.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Restituisce un valore che indica se i nomi delle voci (file) dell'archivio sono crittografati. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Restituisce informazioni sul formato dell'archivio. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Restituisce informazioni sul formato dell'archivio. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Restituisce informazioni sull'istanza dell'archivio. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Restituisce informazioni sull'istanza dell'archivio. |
| [getFormatInfo()](#getFormatInfo--) | Restituisce le informazioni sul formato dell'archivio. |
| [isContentEncrypted()](#isContentEncrypted--) | Restituisce un valore che indica se il contenuto dell'archivio è crittografato. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Restituisce un valore che indica se i nomi delle voci (file) dell'archivio sono crittografati.

**Returns:**
boolean - un valore che indica se i nomi delle voci (file) dell'archivio sono crittografati.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Restituisce informazioni sul formato dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Il flusso del file di archivio. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Restituisce informazioni sul formato dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file di archivio. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Restituisce informazioni sull'istanza dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Il flusso del file di archivio. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Restituisce informazioni sull'istanza dell'archivio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file di archivio. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Restituisce le informazioni sul formato dell'archivio.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Restituisce un valore che indica se il contenuto dell'archivio è crittografato.

**Returns:**
boolean - un valore che indica se il contenuto dell'archivio è crittografato.
