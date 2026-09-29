---
title: "ArchiveInstanceInfo"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αναπαριστά πληροφορίες σχετικά με το στιγμιότυπο του αρχείου."
type: docs
weight: 34
url: /el/java/com.aspose.zip/archiveinstanceinfo/
---

**Inheritance:**
java.lang.Object
```
public final class ArchiveInstanceInfo
```

Αναπαριστά πληροφορίες σχετικά με το στιγμιότυπο του αρχείου.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [areFileNamesEncrypted()](#areFileNamesEncrypted--) | Λαμβάνει μια τιμή που υποδεικνύει εάν τα ονόματα των καταχωρήσεων (αρχείων) της αρχειοθήκης είναι κρυπτογραφημένα. |
| [getArchiveFormatInfo(InputStream stream)](#getArchiveFormatInfo-java.io.InputStream-) | Λαμβάνει πληροφορίες μορφής αρχειοθήκης. |
| [getArchiveFormatInfo(String fileName)](#getArchiveFormatInfo-java.lang.String-) | Λαμβάνει πληροφορίες μορφής αρχειοθήκης. |
| [getArchiveInstanceInfo(InputStream stream)](#getArchiveInstanceInfo-java.io.InputStream-) | Λαμβάνει πληροφορίες στιγμιότυπου αρχειοθήκης. |
| [getArchiveInstanceInfo(String fileName)](#getArchiveInstanceInfo-java.lang.String-) | Λαμβάνει πληροφορίες στιγμιότυπου αρχειοθήκης. |
| [getFormatInfo()](#getFormatInfo--) | Λαμβάνει τις πληροφορίες μορφής της αρχειοθήκης. |
| [isContentEncrypted()](#isContentEncrypted--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το περιεχόμενο του αρχείου είναι κρυπτογραφημένο. |
### areFileNamesEncrypted() {#areFileNamesEncrypted--}
```
public final boolean areFileNamesEncrypted()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν τα ονόματα των καταχωρήσεων (αρχείων) της αρχειοθήκης είναι κρυπτογραφημένα.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν τα ονόματα των καταχωρήσεων (αρχείων) του αρχείου είναι κρυπτογραφημένα.
### getArchiveFormatInfo(InputStream stream) {#getArchiveFormatInfo-java.io.InputStream-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(InputStream stream)
```


Λαμβάνει πληροφορίες μορφής αρχειοθήκης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή του αρχείου αρχειοθήκης. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveFormatInfo(String fileName) {#getArchiveFormatInfo-java.lang.String-}
```
public static ArchiveFormatInfo getArchiveFormatInfo(String fileName)
```


Λαμβάνει πληροφορίες μορφής αρχειοθήκης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το όνομα αρχείου του αρχείου αρχειοθήκης. |

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - Information about archive format.
### getArchiveInstanceInfo(InputStream stream) {#getArchiveInstanceInfo-java.io.InputStream-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(InputStream stream)
```


Λαμβάνει πληροφορίες στιγμιότυπου αρχειοθήκης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή του αρχείου αρχειοθήκης. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getArchiveInstanceInfo(String fileName) {#getArchiveInstanceInfo-java.lang.String-}
```
public static ArchiveInstanceInfo getArchiveInstanceInfo(String fileName)
```


Λαμβάνει πληροφορίες στιγμιότυπου αρχειοθήκης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το όνομα αρχείου του αρχείου αρχειοθήκης. |

**Returns:**
[ArchiveInstanceInfo](../../com.aspose.zip/archiveinstanceinfo) - Information about archive instance or null if format was not detected.
### getFormatInfo() {#getFormatInfo--}
```
public final ArchiveFormatInfo getFormatInfo()
```


Λαμβάνει τις πληροφορίες μορφής της αρχειοθήκης.

**Returns:**
[ArchiveFormatInfo](../../com.aspose.zip/archiveformatinfo) - the archive format info.
### isContentEncrypted() {#isContentEncrypted--}
```
public final boolean isContentEncrypted()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το περιεχόμενο του αρχείου είναι κρυπτογραφημένο.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν το περιεχόμενο του αρχείου είναι κρυπτογραφημένο.
