---
title: SevenZipArchive.SaveSplit
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchive μέθοδος. Αποθηκεύει το αρχείο πολλών τόμων στον παρεχόμενο κατάλογο προορισμού.
type: docs
weight: 90
url: /el/net/aspose.zip.sevenzip/sevenziparchive/savesplit/
---
## SevenZipArchive.SaveSplit method

Αποθηκεύει το αρχείο πολλών τόμων στον παρεχόμενο κατάλογο προορισμού.

```csharp
public void SaveSplit(string destinationDirectory, SplitSevenZipArchiveSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς τον κατάλογο όπου θα δημιουργηθούν τα τμήματα αρχειοθέτησης. |
| options | SplitSevenZipArchiveSaveOptions | Επιλογές για αποθήκευση αρχείου, συμπεριλαμβανομένου του ονόματος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Αυτό το αρχείο άνοιξε από υπάρχουσα πηγή. |
| ArgumentNullException | *destinationDirectory* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης στον κατάλογο. |
| ArgumentException | *destinationDirectory* περιέχει μη έγκυρους χαρακτήρες όπως ", &gt;, &lt; ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή υπερβαίνει το μέγιστο μήκος που καθορίζεται από το σύστημα. |

### Παρατηρήσεις

Αυτή η μέθοδος συνθέτει πολλά (`n`) filename filename.7z.001, filename.7z.002, ..., filename.7z.(n).

Δεν είναι δυνατό να γίνει το υπάρχον αρχείο πολλών τόμων.

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)


