---
title: "Κλάση LhaArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κλάση Aspose.Zip.Lha.LhaArchive. Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LHA .lzh"
type: docs
weight: 630
url: /el/net/aspose.zip.lha/lhaarchive/
---
## LhaArchive class

Αυτή η κλάση αντιπροσωπεύει ένα αρχείο LHA (.lzh).

```csharp
public class LhaArchive : IArchive
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [LhaArchive](lhaarchive/#constructor)(Stream, LhaLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `LhaArchive` και δημιουργεί μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |
| [LhaArchive](lhaarchive/#constructor_1)(string, LhaLoadOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης `LhaArchive` και δημιουργεί μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Entries](../../aspose.zip.lha/lhaarchive/entries/) { get; } | Αποκτά καταχωρίσεις αρχείων τύπου [`LhaArchiveEntry`](../lhaarchiveentry/) που αποτελούν το αρχείο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Dispose](../../aspose.zip.lha/lhaarchive/dispose/)() |  |
| [ExtractToDirectory](../../aspose.zip.lha/lhaarchive/extracttodirectory/)(string) | Εξάγει όλα τα αρχεία και τους καταλόγους στο αρχείο στον παρεχόμενο κατάλογο. |

## Παρατηρήσεις

Μόνο οι ακόλουθες μέθοδοι συμπίεσης υποστηρίζονται:

**Method**

**Explanation**

**lh0**

Ασυμπίεστο

**lh4**

8 KiB κυλιόμενο λεξικό και στατικό Huffman

**lh5**

16 KiB κυλιόμενο λεξικό και στατικό Huffman

**lh6**

64 KiB κυλιόμενο λεξικό και στατικό Huffman

**lh7**

128 KiB κυλιόμενο λεξικό και στατικό Huffman

**lhx**

1 Mib κυλιόμενο λεξικό και στατικό Huffman

**lhd**

Κατάλογος

### Δείτε επίσης

* interface [IArchive](../../aspose.zip/iarchive/)
* namespace [Aspose.Zip.Lha](../../aspose.zip.lha/)
* assembly [Aspose.Zip](../../)


