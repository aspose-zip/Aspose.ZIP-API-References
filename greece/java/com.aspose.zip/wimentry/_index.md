---
title: "WimEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει ένα μεμονωμένο αρχείο ή φάκελο μέσα σε εικόνα wim."
type: docs
weight: 132
url: /el/java/com.aspose.zip/wimentry/
---

**Inheritance:**
java.lang.Object
```
public abstract class WimEntry
```

Αντιπροσωπεύει ένα μεμονωμένο αρχείο ή φάκελο μέσα σε εικόνα wim.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getAlternateDataStreams()](#getAlternateDataStreams--) | Λαμβάνει τα ονόματα των εναλλακτικών ροών δεδομένων για το αρχείο ή τον φάκελο. |
| [getArchive()](#getArchive--) | Λαμβάνει το αρχείο στο οποίο ανήκει η καταχώρηση. |
| [getChangeTime()](#getChangeTime--) | Λαμβάνει την τελευταία φορά που το αρχείο ή ο φάκελος άλλαξε. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει την ώρα δημιουργίας του αρχείου ή του φακέλου. |
| [getFileAttributes()](#getFileAttributes--) | Λαμβάνει τα χαρακτηριστικά του αρχείου ή του φακέλου. |
| [getFullPath()](#getFullPath--) | Λαμβάνει τη πλήρη διαδρομή της καταχώρησης μέσα στην εικόνα. |
| [getHardLink()](#getHardLink--) | Λαμβάνει το αναγνωριστικό hardlink του αρχείου ή του φακέλου. |
| [getImage()](#getImage--) | Λαμβάνει την εικόνα στην οποία ανήκει η καταχώρηση. |
| [getLastAccessTime()](#getLastAccessTime--) | Λαμβάνει την ώρα τελευταίας πρόσβασης του αρχείου ή του φακέλου. |
| [getLastWriteTime()](#getLastWriteTime--) | Λαμβάνει την ώρα τροποποίησης του αρχείου ή του φακέλου. |
| [getModificationTime()](#getModificationTime--) | Λαμβάνει την ώρα τροποποίησης του αρχείου ή του φακέλου. |
| [getName()](#getName--) | Λαμβάνει το όνομα της καταχώρησης μέσα στην εικόνα. |
| [getParent()](#getParent--) | Λαμβάνει τον γονικό φάκελο στον οποίο ανήκει η καταχώρηση. |
| [getShortName()](#getShortName--) | Λαμβάνει το σύντομο όνομα της καταχώρησης μέσα στην εικόνα. |
| [hasHardLinks()](#hasHardLinks--) | Λαμβάνει αν το αρχείο ή ο φάκελος είναι γνωστό με άλλα ονόματα. |
| [isDirectory()](#isDirectory--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο. |
| [toString()](#toString--) | Επιστρέφει την αναπαράσταση ως συμβολοσειρά της παρουσίας της κλάσης [WimEntry](../../com.aspose.zip/wimentry). |
### getAlternateDataStreams() {#getAlternateDataStreams--}
```
public final String[] getAlternateDataStreams()
```


Λαμβάνει τα ονόματα των εναλλακτικών ροών δεδομένων για το αρχείο ή τον φάκελο.

**Returns:**
java.lang.String[] - τα ονόματα των εναλλακτικών ροών δεδομένων για το αρχείο ή τον φάκελο
### getArchive() {#getArchive--}
```
public final WimArchive getArchive()
```


Λαμβάνει το αρχείο στο οποίο ανήκει η καταχώρηση.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the entry belongs to
### getChangeTime() {#getChangeTime--}
```
public final Date getChangeTime()
```


Λαμβάνει την τελευταία φορά που το αρχείο ή ο φάκελος άλλαξε.

**Returns:**
java.util.Date - η τελευταία φορά που το αρχείο ή ο φάκελος άλλαξε
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Λαμβάνει την ώρα δημιουργίας του αρχείου ή του φακέλου.

**Returns:**
java.util.Date - η ώρα δημιουργίας του αρχείου ή του φακέλου
### getFileAttributes() {#getFileAttributes--}
```
public final int getFileAttributes()
```


Λαμβάνει τα χαρακτηριστικά του αρχείου ή του φακέλου.

**Returns:**
int - τα χαρακτηριστικά του αρχείου ή του φακέλου
### getFullPath() {#getFullPath--}
```
public final String getFullPath()
```


Λαμβάνει τη πλήρη διαδρομή της καταχώρησης μέσα στην εικόνα.

**Returns:**
java.lang.String - η πλήρης διαδρομή της καταχώρησης μέσα στην εικόνα
### getHardLink() {#getHardLink--}
```
public final long getHardLink()
```


Λαμβάνει το αναγνωριστικό hardlink του αρχείου ή του φακέλου.

**Returns:**
long - το αναγνωριστικό hardlink του αρχείου ή του φακέλου
### getImage() {#getImage--}
```
public final WimImage getImage()
```


Λαμβάνει την εικόνα στην οποία ανήκει η καταχώρηση.

**Returns:**
[WimImage](../../com.aspose.zip/wimimage) - the image the entry belongs to
### getLastAccessTime() {#getLastAccessTime--}
```
public final Date getLastAccessTime()
```


Λαμβάνει την ώρα τελευταίας πρόσβασης του αρχείου ή του φακέλου.

**Returns:**
java.util.Date - η τελευταία ώρα πρόσβασης του αρχείου ή του φακέλου
### getLastWriteTime() {#getLastWriteTime--}
```
public final Date getLastWriteTime()
```


Λαμβάνει την ώρα τροποποίησης του αρχείου ή του φακέλου.

**Returns:**
java.util.Date - η ώρα τροποποίησης του αρχείου ή του φακέλου
### getModificationTime() {#getModificationTime--}
```
public final Date getModificationTime()
```


Λαμβάνει την ώρα τροποποίησης του αρχείου ή του φακέλου.

**Returns:**
java.util.Date - η ώρα τροποποίησης του αρχείου ή του φακέλου
### getName() {#getName--}
```
public final String getName()
```


Λαμβάνει το όνομα της καταχώρησης μέσα στην εικόνα.

**Returns:**
java.lang.String - το όνομα της καταχώρησης μέσα στην εικόνα
### getParent() {#getParent--}
```
public final WimDirectoryEntry getParent()
```


Λαμβάνει τον γονικό φάκελο στον οποίο ανήκει η καταχώρηση.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the parent directory the entry belongs to
### getShortName() {#getShortName--}
```
public final String getShortName()
```


Λαμβάνει το σύντομο όνομα της καταχώρησης μέσα στην εικόνα.

**Returns:**
java.lang.String - το σύντομο όνομα της καταχώρησης μέσα στην εικόνα
### hasHardLinks() {#hasHardLinks--}
```
public final boolean hasHardLinks()
```


Λαμβάνει αν το αρχείο ή ο φάκελος είναι γνωστό με άλλα ονόματα.

**Returns:**
boolean - αν το αρχείο ή ο φάκελος είναι γνωστό με άλλα ονόματα
### isDirectory() {#isDirectory--}
```
public final boolean isDirectory()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει κατάλογο.

**Returns:**
boolean - μια τιμή που υποδεικνύει αν η καταχώρηση αντιπροσωπεύει κατάλογο
### toString() {#toString--}
```
public String toString()
```


Επιστρέφει την αναπαράσταση ως συμβολοσειρά της παρουσίας της κλάσης [WimEntry](../../com.aspose.zip/wimentry).

**Returns:**
java.lang.String - αναπαράσταση συμβολοσειράς αυτού του αντικειμένου
