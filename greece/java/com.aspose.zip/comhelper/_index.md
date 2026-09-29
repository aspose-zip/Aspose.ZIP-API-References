---
title: "ComHelper"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Παρέχει μεθόδους για πελάτες COM ώστε να φορτώνουν αρχεία στο Aspose.Zip."
type: docs
weight: 55
url: /el/java/com.aspose.zip/comhelper/
---

**Inheritance:**
java.lang.Object
```
public class ComHelper
```

Παρέχει μεθόδους για πελάτες COM ώστε να φορτώνουν αρχεία στο Aspose.Zip.

Χρησιμοποιήστε την κλάση ComHelper για να φορτώσετε ένα αρχείο από αρχείο ή ροή. Ορισμένες κλάσεις παρέχουν έναν προεπιλεγμένο κατασκευαστή για τη δημιουργία νέου αρχείου και επίσης παρέχουν υπερφορτωμένους κατασκευαστές για τη φόρτωση ενός αρχείου από αρχείο ή ροή. Εάν χρησιμοποιείτε Aspose.Zip από εφαρμογή .NET, μπορείτε να χρησιμοποιήσετε απευθείας όλους τους κατασκευαστές αρχείων, αλλά εάν χρησιμοποιείτε Aspose.Zip από εφαρμογή COM, είναι διαθέσιμο μόνο ο προεπιλεγμένος κατασκευαστής αρχείου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ComHelper()](#ComHelper--) | Δημιουργεί μια νέα παρουσία αυτής της κλάσης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [openBzip2(InputStream stream)](#openBzip2-java.io.InputStream-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο bzip2 από ροή. |
| [openBzip2(String fileName)](#openBzip2-java.lang.String-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο bzip2 από αρχείο. |
| [openGzip(InputStream stream)](#openGzip-java.io.InputStream-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο gzip από ροή. |
| [openGzip(String fileName)](#openGzip-java.lang.String-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο gzip από αρχείο. |
| [openRar(InputStream stream)](#openRar-java.io.InputStream-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο rar από ροή. |
| [openRar(String fileName)](#openRar-java.lang.String-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο rar από αρχείο. |
| [openZip(InputStream stream)](#openZip-java.io.InputStream-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο ZIP από ροή. |
| [openZip(String fileName)](#openZip-java.lang.String-) | Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο ZIP από αρχείο. |
### ComHelper() {#ComHelper--}
```
public ComHelper()
```


Δημιουργεί μια νέα παρουσία αυτής της κλάσης.

### openBzip2(InputStream stream) {#openBzip2-java.io.InputStream-}
```
public final Bzip2Archive openBzip2(InputStream stream)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο bzip2 από ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openBzip2(String fileName) {#openBzip2-java.lang.String-}
```
public final Bzip2Archive openBzip2(String fileName)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο bzip2 από αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Όνομα αρχείου του αρχείου προς φόρτωση. |

**Returns:**
[Bzip2Archive](../../com.aspose.zip/bzip2archive) - A [Bzip2Archive](../../com.aspose.zip/bzip2archive) object that represents the archive.
### openGzip(InputStream stream) {#openGzip-java.io.InputStream-}
```
public final GzipArchive openGzip(InputStream stream)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο gzip από ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openGzip(String fileName) {#openGzip-java.lang.String-}
```
public final GzipArchive openGzip(String fileName)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο gzip από αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Όνομα αρχείου του αρχείου προς φόρτωση. |

**Returns:**
[GzipArchive](../../com.aspose.zip/gziparchive) - A [GzipArchive](../../com.aspose.zip/gziparchive) object that represents the archive.
### openRar(InputStream stream) {#openRar-java.io.InputStream-}
```
public final RarArchive openRar(InputStream stream)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο rar από ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openRar(String fileName) {#openRar-java.lang.String-}
```
public final RarArchive openRar(String fileName)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο rar από αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Όνομα αρχείου του αρχείου προς φόρτωση. |

**Returns:**
[RarArchive](../../com.aspose.zip/rararchive) - A [RarArchive](../../com.aspose.zip/rararchive) object that represents the archive.
### openZip(InputStream stream) {#openZip-java.io.InputStream-}
```
public final Archive openZip(InputStream stream)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο ZIP από ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Ένα αντικείμενο ροής .NET που περιέχει το αρχείο προς φόρτωση. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
### openZip(String fileName) {#openZip-java.lang.String-}
```
public final Archive openZip(String fileName)
```


Επιτρέπει σε μια εφαρμογή COM να φορτώσει ένα αρχείο ZIP από αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Όνομα αρχείου του αρχείου προς φόρτωση. |

**Returns:**
[Archive](../../com.aspose.zip/archive) - A [Archive](../../com.aspose.zip/archive) object that represents the archive.
