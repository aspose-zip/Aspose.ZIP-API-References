---
title: "AppleLzmaCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη συμπίεση LZMA μέσα σε αρχείο Apple Archive .aar."
type: docs
weight: 23
url: /el/java/com.aspose.zip/applelzmacompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLzmaCompressionSettings extends AppleCompressionSettings
```

Ρυθμίσεις για τη συμπίεση LZMA μέσα σε ένα αρχείο Apple Archive (.aar).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AppleLzmaCompressionSettings(int blockSize)](#AppleLzmaCompressionSettings-int-) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize)](#AppleLzmaCompressionSettings-int-int-) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)](#AppleLzmaCompressionSettings-int-int-int-) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings). |
| [AppleLzmaCompressionSettings()](#AppleLzmaCompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) με προεπιλεγμένες παραμέτρους. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Λαμβάνει το μέγεθος κάθε μπλοκ δεδομένων πριν από τη συμπίεση. |
| [getDictionarySize()](#getDictionarySize--) | Λαμβάνει το μέγεθος του λεξικού που χρησιμοποιείται για τη συμπίεση. |
| [getFastBytes()](#getFastBytes--) | Λαμβάνει τον αριθμό των γρήγορων byte που χρησιμοποιούνται για τη συμπίεση. |
### AppleLzmaCompressionSettings(int blockSize) {#AppleLzmaCompressionSettings-int-}
```
public AppleLzmaCompressionSettings(int blockSize)
```


Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | int | Το μέγεθος κάθε μπλοκ δεδομένων πριν από τη συμπίεση. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize) {#AppleLzmaCompressionSettings-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize)
```


Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | int | Το μέγεθος κάθε μπλοκ δεδομένων πριν από τη συμπίεση. |
| dictionarySize | int | Το μέγεθος του λεξικού που χρησιμοποιείται για τη συμπίεση. |

### AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes) {#AppleLzmaCompressionSettings-int-int-int-}
```
public AppleLzmaCompressionSettings(int blockSize, int dictionarySize, int fastBytes)
```


Αρχικοποιεί ένα νέο παράδειγμα της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | int | Το μέγεθος κάθε μπλοκ δεδομένων πριν από τη συμπίεση. |
| dictionarySize | int | Το μέγεθος του λεξικού που χρησιμοποιείται για τη συμπίεση. |
| fastBytes | int | Ο αριθμός των γρήγορων byte που χρησιμοποιούνται για τη συμπίεση. |

### AppleLzmaCompressionSettings() {#AppleLzmaCompressionSettings--}
```
public AppleLzmaCompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [AppleLzmaCompressionSettings](../../com.aspose.zip/applelzmacompressionsettings) με προεπιλεγμένες παραμέτρους.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Λαμβάνει το μέγεθος κάθε μπλοκ δεδομένων πριν από τη συμπίεση.

Τιμή: Η προεπιλεγμένη τιμή είναι 4 MiB.

**Returns:**
int - το μέγεθος κάθε μπλοκ δεδομένων πριν από τη συμπίεση.
### getDictionarySize() {#getDictionarySize--}
```
public final int getDictionarySize()
```


Λαμβάνει το μέγεθος του λεξικού που χρησιμοποιείται για τη συμπίεση.

Τιμή: Η προεπιλεγμένη τιμή είναι 8 MiB.

**Returns:**
int - το μέγεθος του λεξικού που χρησιμοποιείται για τη συμπίεση.
### getFastBytes() {#getFastBytes--}
```
public final int getFastBytes()
```


Λαμβάνει τον αριθμό των γρήγορων byte που χρησιμοποιούνται για τη συμπίεση.

Τιμή: Η προεπιλεγμένη τιμή είναι 32.

**Returns:**
int - ο αριθμός των γρήγορων byte που χρησιμοποιούνται για τη συμπίεση.
