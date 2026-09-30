---
title: "SevenZipArchive.SaveSplit"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SevenZipArchive μέθοδος. Αποθηκεύει το πολυτόμο αρχείο στον προορισμένο κατάλογο που παρέχεται."
type: docs
weight: 90
url: /el/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Αποθηκεύει το αρχείο πολλαπλών τόμων στον παρεχόμενο φάκελο προορισμού.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς το φάκελο όπου θα δημιουργηθούν τα τμήματα του αρχείου. |
| επιλογές | SplitSevenZipArchiveSaveOptions | Επιλογές για την αποθήκευση του αρχείου, συμπεριλαμβανομένου του ονόματος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *destinationDirectory* είναι null. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον φάκελο. |
| ArgumentException | *destinationDirectory* περιέχει μη έγκυρους χαρακτήρες όπως \", &gt;, &lt;, ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| EndOfStreamException | Εκτοξεύεται όταν το τέλος της ροής επιτυγχάνεται πριν διαβαστούν ο αριθμός των αναμενόμενων byte. |

## Παρατηρήσεις

Αυτή η μέθοδος συνθέτει πολλά (`n`) αρχεία filename.7z.001, filename.7z.002, ..., filename.7z.(n).

## Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitSevenZipArchiveSaveOptions("volume", 65536));
}
```

### Δείτε επίσης

* class [SplitSevenZipArchiveSaveOptions](../../../aspose.zip.saving/splitsevenziparchivesaveoptions/)
* class [SevenZipArchive](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchive/)
* assembly [Aspose.Zip](../../../)


