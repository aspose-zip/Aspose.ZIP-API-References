---
title: "AlzArchiveLoadOptions"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Επιλογές με τις οποίες ένα αρχείο ALZ φορτώνεται από ένα συμπιεσμένο αρχείο."
type: docs
weight: 12
url: /el/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Επιλογές με τις οποίες ένα αρχείο ALZ φορτώνεται από ένα συμπιεσμένο αρχείο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Λαμβάνει τον κωδικό πρόσβασης που χρησιμοποιείται για την αποκρυπτογράφηση των καταχωρίσεων. |
| [getEncoding()](#getEncoding--) | Λαμβάνει την κωδικοποίηση που χρησιμοποιείται για τα ονόματα των καταχωρίσεων. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Λαμβάνει αν η επαλήθευση του αθροίσματος ελέγχου των καταχωρίσεων ALZ παραλείπεται. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της εξαγωγής. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Ορίζει τον κωδικό πρόσβασης που χρησιμοποιείται για την αποκρυπτογράφηση των καταχωρίσεων. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ορίζει την κωδικοποίηση που χρησιμοποιείται για τα ονόματα των καταχωρίσεων. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Ορίζει αν η επαλήθευση του αθροίσματος ελέγχου των καταχωρίσεων ALZ παραλείπεται. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Λαμβάνει τον κωδικό πρόσβασης που χρησιμοποιείται για την αποκρυπτογράφηση των καταχωρίσεων.

**Returns:**
java.lang.String - κωδικός πρόσβασης που χρησιμοποιείται για την αποκρυπτογράφηση των καταχωρίσεων, ή `null` όταν δεν έχει ρυθμιστεί
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Λαμβάνει την κωδικοποίηση που χρησιμοποιείται για τα ονόματα των καταχωρίσεων. Η προεπιλογή είναι η κορεατική κωδική σελίδα Windows 949 (CP949). Τα αρχεία ALZ αποθηκεύουν ιστορικά τα ονόματα αρχείων χρησιμοποιώντας την κορεατική κωδική σελίδα ANSI των Windows.

**Returns:**
java.nio.charset.Charset - κωδικοποίηση που χρησιμοποιείται για τα ονόματα των καταχωρίσεων
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Λαμβάνει αν η επαλήθευση του αθροίσματος ελέγχου των καταχωρίσεων ALZ παραλείπεται. Η προεπιλογή είναι `false`.

**Returns:**
boolean - αν η επαλήθευση του αθροίσματος ελέγχου παραλείπεται
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ορίζει μια σημαία ακύρωσης που χρησιμοποιείται για την ακύρωση της εξαγωγής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | σημαία ακύρωσης, ή `null` για να απενεργοποιηθεί η ακύρωση |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Ορίζει τον κωδικό πρόσβασης που χρησιμοποιείται για την αποκρυπτογράφηση των καταχωρίσεων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.lang.String | κωδικός πρόσβασης που χρησιμοποιείται για την αποκρυπτογράφηση των καταχωρίσεων |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ορίζει την κωδικοποίηση που χρησιμοποιείται για τα ονόματα των καταχωρίσεων. Τα αρχεία ALZ αποθηκεύουν ιστορικά τα ονόματα αρχείων χρησιμοποιώντας την κορεατική κωδική σελίδα ANSI των Windows.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | java.nio.charset.Charset | κωδικοποίηση που χρησιμοποιείται για τα ονόματα των καταχωρίσεων |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Ορίζει αν η επαλήθευση του αθροίσματος ελέγχου των καταχωρίσεων ALZ παραλείπεται.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | boolean | αν η επαλήθευση του αθροίσματος ελέγχου παραλείπεται |

