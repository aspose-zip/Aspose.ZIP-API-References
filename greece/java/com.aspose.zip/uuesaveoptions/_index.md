---
title: "UueSaveOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για την αποθήκευση ενός αρχείου uuencoded."
type: docs
weight: 129
url: /el/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Επιλογές για την αποθήκευση ενός αρχείου uuencoded.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Αρχικοποιεί τις επιλογές με το όνομα αρχείου που παρέχεται από τον χρήστη και τη νέα γραμμή. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Αρχικοποιεί τις επιλογές με το όνομα αρχείου που παρέχεται από τον χρήστη και τη προεπιλεγμένη νέα γραμμή. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getFileName()](#getFileName--) | Λαμβάνει το όνομα αρχείου που θα χρησιμοποιηθεί κατά την επαναδημιουργία των αποκωδικοποιημένων δεδομένων. |
| [getNewLine()](#getNewLine--) | Λαμβάνει τον χαρακτήρα που τερματίζει κάθε γραμμή, συνήθως "\n" ή "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Λαμβάνει τα δικαιώματα αρχείου Unix του αρχείου. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Ορίζει τα δικαιώματα Unix του αρχείου. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Αρχικοποιεί τις επιλογές με το όνομα αρχείου που παρέχεται από τον χρήστη και τη νέα γραμμή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | το όνομα αρχείου που θα χρησιμοποιηθεί κατά την επαναδημιουργία των αποκωδικοποιημένων δεδομένων |
| newLine | java.lang.String | ο χαρακτήρας που τερματίζει κάθε γραμμή |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Αρχικοποιεί τις επιλογές με το όνομα αρχείου που παρέχεται από τον χρήστη και τη προεπιλεγμένη νέα γραμμή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | το όνομα αρχείου που θα χρησιμοποιηθεί κατά την επαναδημιουργία των αποκωδικοποιημένων δεδομένων |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Λαμβάνει το όνομα αρχείου που θα χρησιμοποιηθεί κατά την επαναδημιουργία των αποκωδικοποιημένων δεδομένων.

**Returns:**
java.lang.String - το όνομα αρχείου που θα χρησιμοποιηθεί κατά την επαναδημιουργία των αποκωδικοποιημένων δεδομένων
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Λαμβάνει τον χαρακτήρα που τερματίζει κάθε γραμμή, συνήθως "\n" ή "\r\n".

**Returns:**
java.lang.String - ο χαρακτήρας που τερματίζει κάθε γραμμή, συνήθως "\n" ή "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Λαμβάνει τα δικαιώματα αρχείου Unix του αρχείου.

Η προεπιλογή είναι 644.

**Returns:**
java.lang.String - τα δικαιώματα Unix του αρχείου
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Ορίζει τα δικαιώματα Unix του αρχείου.

Η προεπιλογή είναι 644.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.lang.String | τα δικαιώματα Unix του αρχείου |

