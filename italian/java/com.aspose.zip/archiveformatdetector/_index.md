---
title: "ArchiveFormatDetector"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Rileva un formato di archivio e fornisce altre informazioni correlate."
type: docs
weight: 32
url: /it/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Rileva un formato di archivio e fornisce altre informazioni correlate.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Inizializza una nuova istanza della classe [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Ottiene le informazioni sul formato. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Ottiene le informazioni sul formato. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Inizializza una nuova istanza della classe [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Ottiene le informazioni sul formato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| flusso | java.io.InputStream | Il flusso del file di archivio. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Ottiene le informazioni sul formato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | Il nome del file di archivio. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
