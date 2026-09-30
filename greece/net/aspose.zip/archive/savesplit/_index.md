---
title: "Archive.SaveSplit"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Archive. Αποθηκεύει αρχείο πολλαπλών τόμων στον παρεχόμενο φάκελο προορισμού."
type: docs
weight: 110
url: /el/net/aspose.zip/archive/savesplit/
---
## SaveSplit(string, SplitArchiveSaveOptions) {#savesplit_1}

Αποθηκεύει το αρχείο πολλαπλών τόμων στον παρεχόμενο φάκελο προορισμού.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destinationDirectory | String | Η διαδρομή προς το φάκελο όπου θα δημιουργηθούν τα τμήματα του αρχείου. |
| επιλογές | SplitArchiveSaveOptions | Επιλογές για την αποθήκευση του αρχείου, συμπεριλαμβανομένου του ονόματος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Αυτό το αρχείο ανοίχθηκε από την υπάρχουσα πηγή. |
| NotSupportedException | Αυτό το αρχείο είναι τόσο συμπιεσμένο με τη μέθοδο XZ όσο και κρυπτογραφημένο. |
| ArgumentNullException | *destinationDirectory* είναι null. |
| SecurityException | Ο καλών δεν διαθέτει τα απαιτούμενα δικαιώματα για πρόσβαση στον φάκελο. |
| ArgumentException | *destinationDirectory* περιέχει μη έγκυρους χαρακτήρες όπως \", &gt;, &lt;, ή &#x7C;. |
| PathTooLongException | Η καθορισμένη διαδρομή υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| DirectoryNotFoundException | Η καθορισμένη διαδρομή είναι μη έγκυρη, όπως όταν βρίσκεται σε μη αντιστοιχισμένο δίσκο. |

## Παρατηρήσεις

Αυτή η μέθοδος συνθέτει πολλά (`n`) αρχεία filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Δεν είναι δυνατόν να μετατραπεί το υπάρχον αρχείο σε πολυτόμες.

## Παραδείγματα

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
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## SaveSplit(IVolumeStreamProvider, SplitArchiveSaveOptions) {#savesplit}

Αποθηκεύει ένα αρχείο πολλαπλών τόμων σε ροές που παρέχονται από έναν πάροχο τόμων.

```csharp
public void SaveSplit(IVolumeStreamProvider volumeStreamProvider, SplitArchiveSaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| volumeStreamProvider | IVolumeStreamProvider | Ο πάροχος των ροών προορισμού για τους τόμους του αρχείου. |
| options | SplitArchiveSaveOptions | Επιλογές για την αποθήκευση του αρχείου. [`FileName`](../../../aspose.zip.saving/splitarchivesaveoptions/filename/) παραβλέπεται. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *volumeStreamProvider* ή *options* είναι null. |
| InvalidOperationException | Αυτό το αρχείο ανοίχτηκε από υπάρχουσα πηγή, ή ο πάροχος επιστρέφει μια null ή μη εγγράψιμη ροή. |
| NotSupportedException | Το αρχείο χρησιμοποιεί συμπίεση XZ. |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |

## Παρατηρήσεις

Οι παρεχόμενες ροές δεν χρειάζεται να υποστηρίζουν αναζήτηση.

Κάθε ολοκληρωμένος τόμος εκκενώνεται, περνάει στο [`VolumeCompleted`](../../../aspose.zip.saving/ivolumestreamprovider/volumecompleted/), και στη συνέχεια διαγράφεται.

Δεν είναι δυνατόν να μετατραπεί ένα υπάρχον αρχείο σε πολυτόμες. Η συμπίεση XZ δεν υποστηρίζεται από αυτήν την υπερφόρτωση επειδή απαιτεί αναζήτηση.

## Παραδείγματα

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(provider,  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Δείτε επίσης

* interface [IVolumeStreamProvider](../../../aspose.zip.saving/ivolumestreamprovider/)
* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


