---
title: "SevenZipCipher"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Βασική κλάση για τον κρυπτογράφο AES που χρησιμοποιείται για κρυπτογράφηση 7-zip."
type: docs
weight: 110
url: /el/java/com.aspose.zip/sevenzipcipher/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Security.Cryptography.ICryptoTransform
```
public abstract class SevenZipCipher implements System.Security.Cryptography.ICryptoTransform
```

Βασική κλάση για τον κρυπτογράφο AES που χρησιμοποιείται για κρυπτογράφηση 7-zip.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [canReuseTransform()](#canReuseTransform--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η τρέχουσα μετατροπή μπορεί να επαναχρησιμοποιηθεί. |
| [canTransformMultipleBlocks()](#canTransformMultipleBlocks--) | Λαμβάνει μια τιμή που υποδεικνύει εάν μπορούν να μετατραπούν πολλαπλά μπλοκ. |
| [dispose()](#dispose--) | Εκτελεί εργασίες που ορίζονται από την εφαρμογή και σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων. |
| [getInputBlockSize()](#getInputBlockSize--) | Λαμβάνει το μέγεθος του μπλοκ εισόδου. |
| [getOutputBlockSize()](#getOutputBlockSize--) | Λαμβάνει το μέγεθος του μπλοκ εξόδου. |
| [transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)](#transformBlock-byte---int-int-byte---int-) | Μετατρέπει την καθορισμένη περιοχή του πίνακα byte εισόδου και αντιγράφει τη δημιουργημένη μετατροπή στην καθορισμένη περιοχή του πίνακα byte εξόδου. |
| [transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)](#transformFinalBlock-byte---int-int-) | Μετατρέπει την καθορισμένη περιοχή του καθορισμένου πίνακα byte. |
### canReuseTransform() {#canReuseTransform--}
```
public abstract boolean canReuseTransform()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η τρέχουσα μετατροπή μπορεί να επαναχρησιμοποιηθεί.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν η τρέχουσα μετατροπή μπορεί να επαναχρησιμοποιηθεί
### canTransformMultipleBlocks() {#canTransformMultipleBlocks--}
```
public abstract boolean canTransformMultipleBlocks()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν μπορούν να μετατραπούν πολλαπλά μπλοκ.

**Returns:**
boolean - μια τιμή που υποδεικνύει εάν μπορούν να μετατραπούν πολλαπλά μπλοκ
### dispose() {#dispose--}
```
public abstract void dispose()
```


Εκτελεί εργασίες που ορίζονται από την εφαρμογή και σχετίζονται με την απελευθέρωση, την αποδέσμευση ή την επαναφορά μη διαχειριζόμενων πόρων.

### getInputBlockSize() {#getInputBlockSize--}
```
public abstract int getInputBlockSize()
```


Λαμβάνει το μέγεθος του μπλοκ εισόδου.

**Returns:**
int - το μέγεθος του μπλοκ εισόδου
### getOutputBlockSize() {#getOutputBlockSize--}
```
public abstract int getOutputBlockSize()
```


Λαμβάνει το μέγεθος του μπλοκ εξόδου.

**Returns:**
int - το μέγεθος του μπλοκ εξόδου
### transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset) {#transformBlock-byte---int-int-byte---int-}
```
public abstract int transformBlock(byte[] inputBuffer, int inputOffset, int inputCount, byte[] outputBuffer, int outputOffset)
```


Μετατρέπει την καθορισμένη περιοχή του πίνακα byte εισόδου και αντιγράφει τη δημιουργημένη μετατροπή στην καθορισμένη περιοχή του πίνακα byte εξόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inputBuffer | byte[] | η είσοδος για την οποία υπολογίζεται η μετατροπή |
| inputOffset | int | η μετατόπιση στον πίνακα byte εισόδου από την οποία αρχίζει η χρήση των δεδομένων |
| inputCount | int | ο αριθμός των byte στον πίνακα byte εισόδου που θα χρησιμοποιηθούν ως δεδομένα |
| outputBuffer | byte[] | η έξοδος στην οποία θα γραφτεί η μετατροπή |
| outputOffset | int | η μετατόπιση στον πίνακα byte εξόδου από την οποία αρχίζει η εγγραφή των δεδομένων |

**Returns:**
int - ο αριθμός των byte που γράφτηκαν
### transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount) {#transformFinalBlock-byte---int-int-}
```
public abstract byte[] transformFinalBlock(byte[] inputBuffer, int inputOffset, int inputCount)
```


Μετατρέπει την καθορισμένη περιοχή του καθορισμένου πίνακα byte.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inputBuffer | byte[] | η είσοδος για την οποία υπολογίζεται η μετατροπή |
| inputOffset | int | η μετατόπιση στον πίνακα byte εισόδου από την οποία αρχίζει η χρήση των δεδομένων |
| inputCount | int | ο αριθμός των byte στον πίνακα byte εισόδου που θα χρησιμοποιηθούν ως δεδομένα |

**Returns:**
byte[] - ο υπολογισμένος μετασχηματισμός
