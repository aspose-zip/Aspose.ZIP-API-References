---
title: "SevenZipPPMdCompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z."
type: docs
weight: 117
url: /el/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Ρυθμίσεις για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z με προεπιλεγμένη σειρά μοντέλου και μέγεθος υπο-κατανεμητή. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Λαμβάνει τη μέγιστη σειρά. |
| [getMethod()](#getMethod--) | Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Λαμβάνει το μέγεθος του υπο-κατανεμητή σε MB. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Δημιουργεί παραδείγματα ρυθμίσεων για τη μέθοδο συμπίεσης PPMd μέσα σε αρχείο 7z.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry("data.bin", "data.bin");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

Η προεπιλεγμένη σειρά μοντέλου είναι 6 και το μέγεθος του υπο-κατανεμητή είναι 16 MB.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Λαμβάνει τη μέγιστη σειρά.

**Returns:**
byte - η μέγιστη σειρά
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Λαμβάνει τη μέθοδο συμπίεσης ή αποσυμπίεσης.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Λαμβάνει το μέγεθος του υπο-κατανεμητή σε MB.

**Returns:**
int - το μέγεθος του υπο-κατανεμητή σε MB
