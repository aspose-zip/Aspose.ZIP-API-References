---
title: "WimImage"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει μια μεμονωμένη εικόνα μέσα σε αρχείο wim."
type: docs
weight: 134
url: /el/java/com.aspose.zip/wimimage/
---

**Inheritance:**
java.lang.Object
```
public final class WimImage
```

Αντιπροσωπεύει μια μεμονωμένη εικόνα μέσα σε αρχείο wim.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία στην εικόνα στον παρεχόμενο φάκελο. |
| [getAllEntries()](#getAllEntries--) | Λαμβάνει τις καταχωρήσεις τύπου [WimEntry](../../com.aspose.zip/wimentry) που αποτελούν την εικόνα αναδρομικά. |
| [getEntry(String path)](#getEntry-java.lang.String-) | Λαμβάνει την καταχώρηση τύπου [WimEntry](../../com.aspose.zip/wimentry) για συγκεκριμένη διαδρομή. |
| [getParent()](#getParent--) | Λαμβάνει το αρχείο στο οποίο ανήκει η εικόνα. |
| [getRootDirectory()](#getRootDirectory--) | Λαμβάνει την καταχώρηση του ριζικού καταλόγου της εικόνας. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία στην εικόνα στον παρεχόμενο φάκελο.

```

``````

try (WimArchive archive = new WimArchive("install.wim")) {
archive.getImages().get_Item(0).extractToDirectory(\"C:\\\\extracted\");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<WimEntry> getAllEntries()
```


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the image recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the image recursively
### getEntry(String path) {#getEntry-java.lang.String-}
```
public final WimEntry getEntry(String path)
```


Gets the entry of [WimEntry](../../com.aspose.zip/wimentry) type for a given path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | the path of file or directory |

**Returns:**
[WimEntry](../../com.aspose.zip/wimentry) - the entry of [WimEntry](../../com.aspose.zip/wimentry) type
### getParent() {#getParent--}
```
public final WimArchive getParent()
```


Gets the archive the image belongs to.

**Returns:**
[WimArchive](../../com.aspose.zip/wimarchive) - the archive the image belongs to
### getRootDirectory() {#getRootDirectory--}
```
public final WimDirectoryEntry getRootDirectory()
```


Gets the root directory entry of the image.

**Returns:**
[WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) - the root directory entry of the image
