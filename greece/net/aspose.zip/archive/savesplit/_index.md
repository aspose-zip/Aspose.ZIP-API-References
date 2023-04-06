---
title: Archive.SaveSplit
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive μέθοδος. Αποθηκεύει το αρχείο πολλών τόμων στον παρεχόμενο κατάλογο προορισμού.
type: docs
weight: 100
url: /el/net/aspose.zip/archive/savesplit/
---
## Archive.SaveSplit method

Αποθηκεύει το αρχείο πολλών τόμων στον παρεχόμενο κατάλογο προορισμού.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς τον κατάλογο όπου θα δημιουργηθούν τα τμήματα αρχειοθέτησης. |
| options | SplitArchiveSaveOptions | Επιλογές για αποθήκευση αρχείου, συμπεριλαμβανομένου του ονόματος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Αυτό το αρχείο άνοιξε από υπάρχουσα πηγή. |
| NotSupportedException | Αυτό το αρχείο είναι συμπιεσμένο με τη μέθοδο XZ και κρυπτογραφημένο. |
| ArgumentNullException | *destinationDirectory* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης στον κατάλογο. |
| ArgumentException | *destinationDirectory* περιέχει μη έγκυρους χαρακτήρες όπως ", &gt;, &lt; ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή υπερβαίνει το μέγιστο μήκος που καθορίζεται από το σύστημα. |

### Παρατηρήσεις

Αυτή η μέθοδος συνθέτει πολλά (`n`) αρχεία filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Δεν είναι δυνατό να γίνει το υπάρχον αρχείο πολλών τόμων.

### Παραδείγματα

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Δείτε επίσης

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


