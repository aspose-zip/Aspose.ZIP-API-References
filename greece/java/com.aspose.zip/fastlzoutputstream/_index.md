---
title: "FastLZOutputStream"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ένα wrapper ροής που συμπιέζει δεδομένα με FastLZ."
type: docs
weight: 68
url: /el/java/com.aspose.zip/fastlzoutputstream/
---

**Inheritance:**
java.lang.Object, java.io.OutputStream
```
public class FastLZOutputStream extends OutputStream
```

Ένα περιτύλιγμα ροής που συμπιέζει δεδομένα με FastLZ. Υλοποιεί το μοτίβο διακοσμητή.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [FastLZOutputStream(OutputStream stream, int compressionLevel)](#FastLZOutputStream-java.io.OutputStream-int-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης FastLZStream προετοιμασμένο για συμπίεση. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [close()](#close--) | Κλείνει την τρέχουσα ροή και απελευθερώνει τυχόν πόρους (όπως υποδοχές και χειριστές αρχείων) που σχετίζονται με την τρέχουσα ροή. |
| [flush()](#flush--) | Καθαρίζει όλες τις προσωρινές μνήμες για αυτή τη ροή και προκαλεί την εγγραφή τυχόν δεδομένων στην υποκείμενη συσκευή. |
| [write(byte[] buffer, int offset, int count)](#write-byte---int-int-) | Γράφει μια ακολουθία byte στη ροή συμπίεσης και προχωρά τη τρέχουσα θέση μέσα σε αυτή τη ροή κατά τον αριθμό των γραμμένων byte. |
| [write(int b)](#write-int-) | Γράφει το καθορισμένο byte σε αυτή τη ροή εξόδου. |
### FastLZOutputStream(OutputStream stream, int compressionLevel) {#FastLZOutputStream-java.io.OutputStream-int-}
```
public FastLZOutputStream(OutputStream stream, int compressionLevel)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης FastLZStream προετοιμασμένο για συμπίεση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | η ροή για αποθήκευση συμπιεσμένων δεδομένων |
| compressionLevel | int | χρησιμοποιήστε 1 για ταχύτερη συμπίεση, χρησιμοποιήστε 2 για καλύτερο λόγο συμπίεσης |

### close() {#close--}
```
public void close()
```


Κλείνει την τρέχουσα ροή και απελευθερώνει τυχόν πόρους (όπως υποδοχές και χειριστές αρχείων) που σχετίζονται με την τρέχουσα ροή.

### flush() {#flush--}
```
public void flush()
```


Καθαρίζει όλες τις προσωρινές μνήμες για αυτή τη ροή και προκαλεί την εγγραφή τυχόν δεδομένων στην υποκείμενη συσκευή.

### write(byte[] buffer, int offset, int count) {#write-byte---int-int-}
```
public void write(byte[] buffer, int offset, int count)
```


Γράφει μια ακολουθία byte στη ροή συμπίεσης και προχωρά τη τρέχουσα θέση μέσα σε αυτή τη ροή κατά τον αριθμό των γραμμένων byte.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| buffer | byte[] | ένας πίνακας byte. Αυτή η μέθοδος αντιγράφει count byte από το buffer στη τρέχουσα ροή |
| offset | int | η μηδενική βάση offset byte στο buffer στην οποία ξεκινά η αντιγραφή byte στη τρέχουσα ροή |
| count | int | ο αριθμός των byte που θα γραφούν στη τρέχουσα ροή |

### write(int b) {#write-int-}
```
public void write(int b)
```


Γράφει το καθορισμένο byte σε αυτή τη ροή εξόδου. Η γενική σύμβαση για το `write` είναι ότι γράφεται ένα byte στη ροή εξόδου. Το byte που θα γραφτεί είναι τα οκτώ χαμηλότερα bits του ορίσματος `b`. Τα 24 υψηλότερα bits του `b` αγνοούνται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| b | int | το `byte` |

