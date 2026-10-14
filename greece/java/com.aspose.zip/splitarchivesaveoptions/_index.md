---
title: "SplitArchiveSaveOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές για την αποθήκευση ενός πολυτόμου αρχείου ZIP."
type: docs
weight: 122
url: /el/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Επιλογές για την αποθήκευση ενός πολυτόμου αρχείου ZIP.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Δημιουργεί ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου ZIP. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Λαμβάνει προαιρετικό σχόλιο για το αρχείο Zip. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Λαμβάνει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης. |
| [getEncoding()](#getEncoding--) | Λαμβάνει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes. |
| [getEventsBag()](#getEventsBag--) | Λαμβάνει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου. |
| [getFileName()](#getFileName--) | Λαμβάνει το όνομα των τμημάτων χωρίς επέκταση. |
| [getSegmentSize()](#getSegmentSize--) | Λαμβάνει το μέγεθος του τμήματος. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Ορίζει προαιρετικό σχόλιο για το αρχείο Zip. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Ορίζει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Δημιουργεί ρυθμίσεις για την αποθήκευση ενός πολυτόμου αρχείου ZIP.

Ορισμένοι τόμοι μπορεί να είναι μικρότεροι από το `segmentSize`. Στις περισσότερες περιπτώσεις, το τελευταίο τμήμα θα είναι μικρότερο, αλλά σπάνια τα κανονικά τμήματα μπορεί επίσης να είναι.

Τα ονόματα των αρχείων θα είναι ως εξής: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Όνομα για τους τόμους. Μπορεί να είναι με ή χωρίς την επέκταση .zip. |
| segmentSize | long | Μέγεθος του τόμου. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Λαμβάνει προαιρετικό σχόλιο για το αρχείο Zip.

**Returns:**
java.lang.String - προαιρετικό σχόλιο για το αρχείο Zip.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Λαμβάνει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes.

Εάν δεν οριστεί, θα χρησιμοποιηθεί η κωδικοσελίδα 437.

**Returns:**
java.nio.charset.Charset - κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Λαμβάνει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Λαμβάνει το όνομα των τμημάτων χωρίς επέκταση.

**Returns:**
java.lang.String - το όνομα των τμημάτων χωρίς επέκταση.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Λαμβάνει το μέγεθος του τμήματος.

**Returns:**
long - το μέγεθος του τμήματος.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Ορίζει προαιρετικό σχόλιο για το αρχείο Zip.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.lang.String | προαιρετικό σχόλιο για το αρχείο Zip. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | μια τιμή που υποδεικνύει εάν οι πηγές των καταχωρήσεων πρέπει να κλείσουν αμέσως μετά τη συμπίεση μιας καταχώρησης. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ορίζει κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε bytes.

Εάν δεν οριστεί, θα χρησιμοποιηθεί η κωδικοσελίδα 437.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.nio.charset.Charset | κωδικοποίηση για τη μετατροπή ονομάτων αρχείων και άλλων συμβολοσειρών σε byte. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Ορίζει το δοχείο των γεγονότων που ενεργοποιούνται κατά την αποθήκευση του αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | υποδοχέας των γεγονότων που δημιουργούνται κατά την αποθήκευση του αρχείου. |

