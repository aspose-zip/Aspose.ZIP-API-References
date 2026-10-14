---
title: "AppleLz4CompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για συμπίεση LZ4 σε αρχείο Apple Archive .aar."
type: docs
weight: 21
url: /el/java/com.aspose.zip/applelz4compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.AppleCompressionSettings](../../com.aspose.zip/applecompressionsettings)
```
public class AppleLz4CompressionSettings extends AppleCompressionSettings
```

Ρυθμίσεις για τη συμπίεση LZ4 μέσα σε ένα αρχείο Apple Archive (.aar).
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AppleLz4CompressionSettings(int blockSize)](#AppleLz4CompressionSettings-int-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings). |
| [AppleLz4CompressionSettings()](#AppleLz4CompressionSettings--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) με προεπιλεγμένες παραμέτρους. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Λαμβάνει το μέγεθος κάθε συμπιεσμένου μπλοκ `pbz4`/`bv41`. |
### AppleLz4CompressionSettings(int blockSize) {#AppleLz4CompressionSettings-int-}
```
public AppleLz4CompressionSettings(int blockSize)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | int | Το μέγεθος κάθε συμπιεσμένου μπλοκ `pbz4`/`bv41`. |

### AppleLz4CompressionSettings() {#AppleLz4CompressionSettings--}
```
public AppleLz4CompressionSettings()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [AppleLz4CompressionSettings](../../com.aspose.zip/applelz4compressionsettings) με προεπιλεγμένες παραμέτρους.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Λαμβάνει το μέγεθος κάθε συμπιεσμένου μπλοκ `pbz4`/`bv41`.

Τιμή: Η προεπιλεγμένη τιμή είναι 4 MiB.

**Returns:**
int - το μέγεθος κάθε συμπιεσμένου μπλοκ `pbz4`/`bv41`.
