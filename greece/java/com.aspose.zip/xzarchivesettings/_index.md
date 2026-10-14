---
title: "XzArchiveSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Η κλάση περιέχει ένα σύνολο ρυθμίσεων για συγκεκριμένη αρχειοθήκη xz."
type: docs
weight: 147
url: /el/java/com.aspose.zip/xzarchivesettings/
---

**Inheritance:**
java.lang.Object
```
public class XzArchiveSettings
```

Η κλάση περιέχει ένα σύνολο ρυθμίσεων για συγκεκριμένη αρχειοθήκη xz.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XzArchiveSettings()](#XzArchiveSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) χρησιμοποιώντας μονή συμπίεση LZMA2. |
| [XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)](#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με προσαρμοσμένες παραμέτρους. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompressionThreads()](#getCompressionThreads--) | Λαμβάνει τον αριθμό των νημάτων συμπίεσης. |
| [getFastSpeed()](#getFastSpeed--) | Λαμβάνει την παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με μέγεθος λεξικού ίσο με 1 megabyte στο φίλτρο LZMA2, μέγεθος μπλοκ ίσο με 4 megabytes και άθροισμα ελέγχου CRC32. |
| [getFastestSpeed()](#getFastestSpeed--) | Λαμβάνει την παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με μέγεθος λεξικού ίσο με 65536 bytes στο φίλτρο LZMA2, μέγεθος μπλοκ ίσο με 1 megabyte και άθροισμα ελέγχου CRC32. |
| [getHighCompression()](#getHighCompression--) | Λαμβάνει την παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με μέγεθος λεξικού ίσο με 32 megabytes στο φίλτρο LZMA2, μέγεθος μπλοκ ίσο με 128 megabytes και άθροισμα ελέγχου CRC32. |
| [getMaximumCompression()](#getMaximumCompression--) | Λαμβάνει την παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με μέγεθος λεξικού ίσο με 64 megabytes στο φίλτρο LZMA2, μέγεθος μπλοκ ίσο με 256 megabytes και άθροισμα ελέγχου CRC32. |
| [getNormal()](#getNormal--) | Λαμβάνει την παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με μέγεθος λεξικού ίσο με 16 megabytes στο φίλτρο LZMA2, μέγεθος μπλοκ ίσο με 64 megabytes και άθροισμα ελέγχου CRC32. |
| [setCompressionThreads(int value)](#setCompressionThreads-int-) | Ορίζει τον αριθμό των νημάτων συμπίεσης. |
### XzArchiveSettings() {#XzArchiveSettings--}
```
public XzArchiveSettings()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) χρησιμοποιώντας μονή συμπίεση LZMA2.

Το προεπιλεγμένο λεξικό στο φίλτρο LZMA2 έχει μέγεθος 16 megabytes, το προεπιλεγμένο μέγεθος μπλοκ είναι 64 megabytes, ο προεπιλεγμένος τύπος αθροίσματος ελέγχου είναι CRC32.

### XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType) {#XzArchiveSettings-com.aspose.zip.XzFilterSettings---long-com.aspose.zip.XzCheckType-}
```
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) με προσαρμοσμένες παραμέτρους.

```

``````

try (FileOutputStream xzFile = new FileOutputStream(\"archive.xz\")) {
XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
try (XzArchive archive = new XzArchive(settings)) {
archive.setSource("data.bin");
archive.save(xzFile);
}
} catch (IOException ex) {
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [XzFilterSettings\[\]](../../com.aspose.zip/xzfiltersettings) | filters (compressors) to be sequentially applied to create [XzArchive](../../com.aspose.zip/xzarchive). It can be either single [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) or pair of [XzBcjX86FilterSettings](../../com.aspose.zip/xzbcjx86filtersettings) and [XzLZMA2FilterSettings](../../com.aspose.zip/xzlzma2filtersettings) |
| blockSize | long | size xz archive block |
| checkType | [XzCheckType](../../com.aspose.zip/xzchecktype) | type of checksum calculation for uncompressed data |

### getCompressionThreads() {#getCompressionThreads--}
```
public final int getCompressionThreads()
```


Gets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Returns:**
int - compression thread count.
### getFastSpeed() {#getFastSpeed--}
```
public static XzArchiveSettings getFastSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 1 megabyte in LZMA2 filter, block size equals to 4 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fast speed
### getFastestSpeed() {#getFastestSpeed--}
```
public static XzArchiveSettings getFastestSpeed()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 65536 bytes in LZMA2 filter, block size equals to 1 megabyte and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the fastest speed
### getHighCompression() {#getHighCompression--}
```
public static XzArchiveSettings getHighCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 32 megabytes in LZMA2 filter, block size equals to 128 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the high compression
### getMaximumCompression() {#getMaximumCompression--}
```
public static XzArchiveSettings getMaximumCompression()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 64 megabytes in LZMA2 filter, block size equals to 256 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with parameters for the maximum compression
### getNormal() {#getNormal--}
```
public static XzArchiveSettings getNormal()
```


Gets the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with dictionary size equals to 16 megabytes in LZMA2 filter, block size equals to 64 megabytes and CRC32 checksum.

**Returns:**
[XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) - the instance of the [XzArchiveSettings](../../com.aspose.zip/xzarchivesettings) class with normal parameters
### setCompressionThreads(int value) {#setCompressionThreads-int-}
```
public final void setCompressionThreads(int value)
```


Sets compression thread count. If the value is greater than 1, multithreading compression will be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | compression thread count.

Do not set this number more than CPU cores |

