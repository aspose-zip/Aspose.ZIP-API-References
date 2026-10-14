---
title: "ArchiveFormatDetector"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ανιχνεύει μια μορφή αρχείου και παρέχει άλλες σχετικές πληροφορίες."
type: docs
weight: 32
url: /el/java/com.aspose.zip/archiveformatdetector/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveFormatDetector
```

Ανιχνεύει μια μορφή αρχείου και παρέχει άλλες σχετικές πληροφορίες.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ArchiveFormatDetector()](#ArchiveFormatDetector--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getFormatInfo(InputStream stream)](#getFormatInfo-java.io.InputStream-) | Λαμβάνει πληροφορίες μορφής. |
| [getFormatInfo(String fileName)](#getFormatInfo-java.lang.String-) | Λαμβάνει πληροφορίες μορφής. |
### ArchiveFormatDetector() {#ArchiveFormatDetector--}
```
public ArchiveFormatDetector()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [ArchiveFormatDetector](../../com.aspose.zip/archiveformatdetector).

### getFormatInfo(InputStream stream) {#getFormatInfo-java.io.InputStream-}
```
public final ArchiveFormatInfo getFormatInfo(InputStream stream)
```


Λαμβάνει πληροφορίες μορφής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή του αρχείου αρχειοθήκης. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
### getFormatInfo(String fileName) {#getFormatInfo-java.lang.String-}
```
public final ArchiveFormatInfo getFormatInfo(String fileName)
```


Λαμβάνει πληροφορίες μορφής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το όνομα αρχείου του αρχείου αρχειοθήκης. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format or null if a format was not detected.
