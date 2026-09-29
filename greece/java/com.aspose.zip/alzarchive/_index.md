---
title: "AlzArchive"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά ένα αρχείο ALZ."
type: docs
weight: 11
url: /el/java/com.aspose.zip/alzarchive/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.zip.IArchive](../../com.aspose.zip/iarchive), java.lang.AutoCloseable
```
public class AlzArchive implements IArchive, AutoCloseable
```

Αντιπροσωπεύει ένα αρχείο ALZ. Χρησιμοποιήστε αυτήν την κλάση για να επιθεωρήσετε και να εξάγετε αρχεία ALZ.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AlzArchive(InputStream stream)](#AlzArchive-java.io.InputStream-) | Αρχικοποιεί ένα αρχείο ALZ από μια ροή. |
| [AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-) | Αρχικοποιεί ένα αρχείο ALZ από μια ροή χρησιμοποιώντας τις παρεχόμενες επιλογές φόρτωσης. |
| [AlzArchive(String filePath)](#AlzArchive-java.lang.String-) | Αρχικοποιεί ένα αρχείο ALZ από μια διαδρομή αρχείου. |
| [AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)](#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-) | Αρχικοποιεί ένα αρχείο ALZ από μια διαδρομή αρχείου χρησιμοποιώντας τις παρεχόμενες επιλογές φόρτωσης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | Απελευθερώνει τους πόρους που κρατούνται από αυτό το αρχείο. |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία και τους καταλόγους στον παρεχόμενο κατάλογο. |
| [getEntries()](#getEntries--) | Αποκτά τις καταχωρήσεις που αποτελούν αυτό το αρχείο. |
| [getFileEntries()](#getFileEntries--) | Αποκτά καταχωρήσεις μέσω της κοινής διεπαφής αρχείου. |
| [getFormat()](#getFormat--) | Αποκτά τη μορφή του αρχείου. |
### AlzArchive(InputStream stream) {#AlzArchive-java.io.InputStream-}
```
public AlzArchive(InputStream stream)
```


Αρχικοποιεί ένα αρχείο ALZ από μια ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Ροή αρχείου ALZ; πρέπει να υποστηρίζει ανάγνωση και αναζήτηση |

### AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.io.InputStream-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(InputStream stream, AlzArchiveLoadOptions loadOptions)
```


Αρχικοποιεί ένα αρχείο ALZ από μια ροή χρησιμοποιώντας τις παρεχόμενες επιλογές φόρτωσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Ροή αρχείου ALZ; πρέπει να υποστηρίζει ανάγνωση και αναζήτηση |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | επιλογές που χρησιμοποιούνται για τη φόρτωση του αρχείου |

### AlzArchive(String filePath) {#AlzArchive-java.lang.String-}
```
public AlzArchive(String filePath)
```


Αρχικοποιεί ένα αρχείο ALZ από μια διαδρομή αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | διαδρομή προς ένα αρχείο ALZ |

### AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions) {#AlzArchive-java.lang.String-com.aspose.zip.AlzArchiveLoadOptions-}
```
public AlzArchive(String filePath, AlzArchiveLoadOptions loadOptions)
```


Αρχικοποιεί ένα αρχείο ALZ από μια διαδρομή αρχείου χρησιμοποιώντας τις παρεχόμενες επιλογές φόρτωσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | διαδρομή προς ένα αρχείο ALZ |
| loadOptions | [AlzArchiveLoadOptions](../../com.aspose.zip/alzarchiveloadoptions) | επιλογές που χρησιμοποιούνται για τη φόρτωση του αρχείου |

### close() {#close--}
```
public void close()
```


Απελευθερώνει τους πόρους που κρατούνται από αυτό το αρχείο.

### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία και τους καταλόγους στον παρεχόμενο κατάλογο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | java.lang.String | κατάλογος προορισμού· δημιουργείται όταν είναι απαραίτητο |

### getEntries() {#getEntries--}
```
public final List<AlzEntry> getEntries()
```


Αποκτά τις καταχωρήσεις που αποτελούν αυτό το αρχείο.

**Returns:**
java.util.List&lt;com.aspose.zip.AlzEntry&gt; - αμετάβλητη λίστα των καταχωρήσεων ALZ
### getFileEntries() {#getFileEntries--}
```
public final Iterable<IArchiveFileEntry> getFileEntries()
```


Αποκτά καταχωρήσεις μέσω της κοινής διεπαφής αρχείου.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.IArchiveFileEntry&gt; - καταχωρήσεις αρχείου
### getFormat() {#getFormat--}
```
public final ArchiveFormat getFormat()
```


Αποκτά τη μορφή του αρχείου.

**Returns:**
[ArchiveFormat](../../com.aspose.zip/archiveformat) - [ArchiveFormat.Alz](../../com.aspose.zip/archiveformat\#Alz)
