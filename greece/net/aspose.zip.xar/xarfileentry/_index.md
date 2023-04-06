---
title: Class XarFileEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: Aspose.Zip.Xar.XarFileEntry τάξη. Αντιπροσωπεύει την καταχώριση αρχείου μέσα στο αρχείο xar.
type: docs
weight: 840
url: /el/net/aspose.zip.xar/xarfileentry/
---
## XarFileEntry class

Αντιπροσωπεύει την καταχώριση αρχείου μέσα στο αρχείο xar.

```csharp
public abstract class XarFileEntry : XarEntry, IArchiveFileEntry
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [CreationTime](../../aspose.zip.xar/xarentry/creationtime/) { get; } | Λαμβάνει το χρόνο δημιουργίας του αρχείου ή του καταλόγου. |
| [FullPath](../../aspose.zip.xar/xarentry/fullpath/) { get; } | Λαμβάνει την πλήρη διαδρομή της καταχώρησης μέσα στο αρχείο. |
| [IsDirectory](../../aspose.zip.xar/xarentry/isdirectory/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν η καταχώρηση αντιπροσωπεύει τον κατάλογο. |
| [LastAccessTime](../../aspose.zip.xar/xarentry/lastaccesstime/) { get; } | Λαμβάνει τον τελευταίο χρόνο πρόσβασης του αρχείου ή του καταλόγου. |
| [LastWriteTime](../../aspose.zip.xar/xarentry/lastwritetime/) { get; } | Λαμβάνει το χρόνο τροποποίησης του αρχείου ή του καταλόγου. |
| abstract [Length](../../aspose.zip.xar/xarfileentry/length/) { get; } | Λαμβάνει το μήκος της καταχώρισης σε byte. |
| [Name](../../aspose.zip.xar/xarentry/name/) { get; } | Λαμβάνει το όνομα της καταχώρησης μέσα στο αρχείο. |
| [Parent](../../aspose.zip.xar/xarentry/parent/) { get; } | Λαμβάνει τον γονικό κατάλογο στον οποίο ανήκει η καταχώρηση. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract_1)(Stream) | Εξάγει την καταχώρηση στη ροή που παρέχεται. |
| abstract [Extract](../../aspose.zip.xar/xarfileentry/extract/#extract)(string) | Εξάγει την καταχώρηση στο σύστημα αρχείων από τη διαδρομή που παρέχεται. |
| abstract [Open](../../aspose.zip.xar/xarfileentry/open/)() | Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με περιεχόμενο καταχώρισης. |
| override [ToString](../../aspose.zip.xar/xarentry/tostring/)() |  |

### Δείτε επίσης

* class [XarEntry](../xarentry/)
* interface [IArchiveFileEntry](../../aspose.zip/iarchivefileentry/)
* χώρος ονομάτων [Aspose.Zip.Xar](../../aspose.zip.xar/)
* συνέλευση [Aspose.Zip](../../)


