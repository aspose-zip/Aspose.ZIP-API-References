---
title: "SevenZipBZip2CompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη μέθοδο συμπίεσης BZip2 μέσα σε αρχείο 7z."
type: docs
weight: 109
url: /el/java/com.aspose.zip/sevenzipbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public class SevenZipBZip2CompressionSettings extends SevenZipCompressionSettings
```

Ρυθμίσεις για τη μέθοδο συμπίεσης BZip2 μέσα σε αρχείο 7z.

Το Bzip2 συμπιέζει αρχεία χρησιμοποιώντας τον αλγόριθμο συμπίεσης κειμένου με ταξινόμηση μπλοκ Burrows-Wheeler και την κωδικοποίηση Huffman.

Δείτε περισσότερα: [Bzip2][]


[Bzip2]: https://en.wikipedia.org/wiki/Bzip2
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SevenZipBZip2CompressionSettings(int blockSize)](#SevenZipBZip2CompressionSettings-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings). |
| [SevenZipBZip2CompressionSettings()](#SevenZipBZip2CompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Μέγεθος μπλοκ σε εκατοντάδες kilobytes. |
| [getMethod()](#getMethod--) | Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης. |
### SevenZipBZip2CompressionSettings(int blockSize) {#SevenZipBZip2CompressionSettings-int-}
```
public SevenZipBZip2CompressionSettings(int blockSize)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | int | μέγεθος μπλοκ σε εκατοντάδες kilobytes |

### SevenZipBZip2CompressionSettings() {#SevenZipBZip2CompressionSettings--}
```
public SevenZipBZip2CompressionSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [SevenZipBZip2CompressionSettings](../../com.aspose.zip/sevenzipbzip2compressionsettings) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Μέγεθος μπλοκ σε εκατοντάδες kilobytes.

**Returns:**
int - μέγεθος μπλοκ σε εκατοντάδες kilobytes
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
