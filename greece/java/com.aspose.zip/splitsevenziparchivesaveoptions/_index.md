---
title: "SplitSevenZipArchiveSaveOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για την αποθήκευση ενός πολυτόμου αρχείου 7-zip."
type: docs
weight: 123
url: /el/java/com.aspose.zip/splitsevenziparchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitSevenZipArchiveSaveOptions
```

Επιλογές για την αποθήκευση ενός πολυτόμου αρχείου 7-zip.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)](#SplitSevenZipArchiveSaveOptions-java.lang.String-long-) | Δημιουργεί ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου 7z. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getFileName()](#getFileName--) | Λαμβάνει το όνομα των τμημάτων χωρίς επέκταση. |
| [getSegmentSize()](#getSegmentSize--) | Λαμβάνει το μέγεθος του τμήματος. |
### SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize) {#SplitSevenZipArchiveSaveOptions-java.lang.String-long-}
```
public SplitSevenZipArchiveSaveOptions(String fileName, long segmentSize)
```


Δημιουργεί ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου 7z.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fileName | java.lang.String | Όνομα για τους τόμους. Μπορεί να είναι με ή χωρίς την επέκταση .7z. |

Τα ονόματα των αρχείων θα είναι ως εξής: `fileName`.7z.001, `fileName`.7z.002, ..., `fileName`.7z.(n). |
|  | segmentSize | long | μέγεθος του τόμου. |

Κάποιοι τόμοι μπορεί να είναι μικρότεροι από το `segmentSize`. Στις περισσότερες περιπτώσεις, το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια τα κανονικά τμήματα μπορεί επίσης να είναι. |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Λαμβάνει το όνομα των τμημάτων χωρίς επέκταση.

**Returns:**
java.lang.String - το όνομα των τμημάτων χωρίς επέκταση
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Λαμβάνει το μέγεθος του τμήματος.

**Returns:**
long - το μέγεθος του τμήματος.
