---
title: "XarDirectoryEntry"
second_title: "Αναφορά API του Aspose.ZIP για Java"
description: "Αντιπροσωπεύει καταχώρηση φακέλου μέσα σε αρχείο xar."
type: docs
weight: 139
url: /el/java/com.aspose.zip/xardirectoryentry/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.XarEntry](../../com.aspose.zip/xarentry)
```
public final class XarDirectoryEntry extends XarEntry
```

Αντιπροσωπεύει καταχώρηση φακέλου μέσα σε αρχείο xar.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [extractToDirectory(String destinationDirectory)](#extractToDirectory-java.lang.String-) | Εξάγει όλα τα αρχεία στον τρέχοντα φάκελο στον παρεχόμενο φάκελο. |
| [getAllEntries()](#getAllEntries--) | Λαμβάνει όλες τις καταχωρήσεις τύπου [XarEntry](../../com.aspose.zip/xarentry) που αποτελούν τον φάκελο αναδρομικά. |
| [getDirectories()](#getDirectories--) | Λαμβάνει καταχωρήσεις τύπου [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) που αποτελούν τον κατάλογο. |
| [getFiles()](#getFiles--) | Λαμβάνει καταχωρήσεις τύπου [XarFileEntry](../../com.aspose.zip/xarfileentry) που αποτελούν τον κατάλογο. |
| [getFilesAndDirectories()](#getFilesAndDirectories--) | Λαμβάνει καταχωρήσεις τύπου [XarEntry](../../com.aspose.zip/xarentry) που αποτελούν τον κατάλογο. |
### extractToDirectory(String destinationDirectory) {#extractToDirectory-java.lang.String-}
```
public final void extractToDirectory(String destinationDirectory)
```


Εξάγει όλα τα αρχεία στον τρέχοντα φάκελο στον παρεχόμενο φάκελο.

```

``````

try (XarArchive archive = new XarArchive("archive.xar")) {
((XarDirectoryEntry)archive.getEntries().get(0)).extractToDirectory("C:\\extracted");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| destinationDirectory | java.lang.String | the path to the directory to place the extracted files in.

If the directory does not exist, it will be created |

### getAllEntries() {#getAllEntries--}
```
public final Iterable<XarEntry> getAllEntries()
```


Gets all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - all entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory recursively
### getDirectories() {#getDirectories--}
```
public final Iterable<XarDirectoryEntry> getDirectories()
```


Gets entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarDirectoryEntry&gt; - entries of [XarDirectoryEntry](../../com.aspose.zip/xardirectoryentry) type constituting the directory
### getFiles() {#getFiles--}
```
public final Iterable<XarFileEntry> getFiles()
```


Gets entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarFileEntry&gt; - entries of [XarFileEntry](../../com.aspose.zip/xarfileentry) type constituting the directory
### getFilesAndDirectories() {#getFilesAndDirectories--}
```
public final Iterable<XarEntry> getFilesAndDirectories()
```


Gets entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory.

**Returns:**
java.lang.Iterable&lt;com.aspose.zip.XarEntry&gt; - entries of [XarEntry](../../com.aspose.zip/xarentry) type constituting the directory
