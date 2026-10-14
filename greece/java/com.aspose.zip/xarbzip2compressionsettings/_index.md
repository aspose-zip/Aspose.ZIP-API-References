---
title: "XarBzip2CompressionSettings"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Ρυθμίσεις για τη μέθοδο συμπίεσης Bzip2."
type: docs
weight: 137
url: /el/java/com.aspose.zip/xarbzip2compressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarCompressionSettings](../../com.aspose.zip/xarcompressionsettings)
```
public class XarBzip2CompressionSettings extends XarCompressionSettings
```

Ρυθμίσεις για τη μέθοδο συμπίεσης Bzip2.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [XarBzip2CompressionSettings(int blockSize)](#XarBzip2CompressionSettings-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings). |
| [XarBzip2CompressionSettings()](#XarBzip2CompressionSettings--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBlockSize()](#getBlockSize--) | Μέγεθος μπλοκ σε εκατοντάδες kilobytes. |
### XarBzip2CompressionSettings(int blockSize) {#XarBzip2CompressionSettings-int-}
```
public XarBzip2CompressionSettings(int blockSize)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings).

```

``````

try (XarArchive archive = new XarArchive()) {
archive.createEntry("data.bin", "data.bin", false, new XarBzip2CompressionSettings(1));
archive.save("archive.xar");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| blockSize | int | block size in hundreds of kilobytes |

### XarBzip2CompressionSettings() {#XarBzip2CompressionSettings--}
```
public XarBzip2CompressionSettings()
```


Initializes a new instance of the [XarBzip2CompressionSettings](../../com.aspose.zip/xarbzip2compressionsettings) class with default block size, equals to 9 hundred of kilobytes.

### getBlockSize() {#getBlockSize--}
```
public final int getBlockSize()
```


Block size in hundreds of kilobytes.

**Returns:**
int - block size in hundreds of kilobytes
