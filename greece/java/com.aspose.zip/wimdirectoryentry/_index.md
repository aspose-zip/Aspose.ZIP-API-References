---
title: "WimDirectoryEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει έναν μεμονωμένο φάκελο μέσα σε αρχείο wim."
type: docs
weight: 131
url: /el/java/com.aspose.zip/wimdirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.WimEntry](../../com.aspose.zip/wimentry)
```
public final class WimDirectoryEntry extends WimEntry
```

Αντιπροσωπεύει έναν μεμονωμένο φάκελο μέσα σε αρχείο wim.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία στον τρέχοντα φάκελο στον παρεχόμενο φάκελο. |
| [getAllEntries()](#getAllEntries--) | Λαμβάνει όλες τις καταχωρήσεις τύπου [WimEntry](../../com.aspose.zip/wimentry) που αποτελούν τον κατάλογο αναδρομικά. |
| [getDirectories()](#getDirectories--) | Λαμβάνει τις καταχωρήσεις τύπου [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) που αποτελούν τον κατάλογο. |
| [getFiles()](#getFiles--) | Λαμβάνει τις καταχωρήσεις τύπου [WimFileEntry](../../com.aspose.zip/wimfileentry) που αποτελούν τον κατάλογο. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Λαμβάνει τις καταχωρήσεις τύπου [WimEntry](../../com.aspose.zip/wimentry) που αποτελούν τον κατάλογο. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία στον τρέχοντα φάκελο στον παρεχόμενο φάκελο.

```

``````

try (WimArchive archive = new WimArchive("archive.wim")) {
archive.getImages().get_Item(0).getRootDirectory().extractToDirectory("C:\\extracted");
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


Gets all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - all entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final List<WimDirectoryEntry> getDirectories()
```


Gets entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimDirectoryEntry&gt; - entries of [WimDirectoryEntry](../../com.aspose.zip/wimdirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final List<WimFileEntry> getFiles()
```


Gets entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory.

**Returns:**
java.util.List&lt;com.aspose.zip.WimFileEntry&gt; - entries of [WimFileEntry](../../com.aspose.zip/wimfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<WimEntry> getFilesAndDirectories()
```


Gets entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.WimEntry&gt; - entries of [WimEntry](../../com.aspose.zip/wimentry) type constituting the directory
