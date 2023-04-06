---
title: SevenZipArchive.SevenZipArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουSevenZipArchive τάξη με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της.
type: docs
weight: 10
url: /el/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`SevenZipArchive`](../) τάξη με προαιρετικές ρυθμίσεις για τις καταχωρήσεις της.

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | Ρυθμίσεις συμπίεσης και κρυπτογράφησης που χρησιμοποιούνται για τις νέες προσθήκες[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) αντικείμενα. Εάν δεν καθορίζεται, θα χρησιμοποιηθεί συμπίεση LZMA χωρίς κρυπτογράφηση. |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να συμπιέσετε ένα μεμονωμένο αρχείο με προεπιλεγμένες ρυθμίσεις: Συμπίεση LZMA χωρίς κρυπτογράφηση.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### Δείτε επίσης

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`SevenZipArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public SevenZipArchive(Stream sourceStream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *sourceStream* δεν είναι αναζητήσιμο. |
| ArgumentNullException | *sourceStream* είναι μηδενικό. |
| NotImplementedException | Το αρχείο περιέχει περισσότερους από έναν κωδικοποιητές. Τώρα υποστηρίζεται μόνο συμπίεση LZMA. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Βλέπω[`ExtractToDirectory`](../extracttodirectory/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`SevenZipArchive`](../) Η λίστα καταχωρήσεων κλάσης και σύνθεσης μπορεί να εξαχθεί από το αρχείο.

```csharp
public SevenZipArchive(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η πλήρως πιστοποιημένη ή η σχετική διαδρομή προς το αρχείο αρχειοθέτησης. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *path* είναι μηδενικό. |
| SecurityException | Ο καλών δεν έχει την απαιτούμενη άδεια πρόσβασης. |
| ArgumentException | ο*path* είναι κενό, περιέχει μόνο λευκά κενά ή περιέχει μη έγκυρους χαρακτήρες. |
| UnauthorizedAccessException | Πρόσβαση στο αρχείο*path* απορρίπτεται. |
| PathTooLongException | Το καθορισμένο*path*, όνομα αρχείου ή και τα δύο υπερβαίνουν το μέγιστο μήκος που καθορίζεται από το σύστημα. Για παράδειγμα, σε πλατφόρμες που βασίζονται σε Windows, οι διαδρομές πρέπει να είναι μικρότερες από 248 χαρακτήρες και τα ονόματα αρχείων πρέπει να είναι λιγότερο από 260 χαρακτήρες. |
| NotSupportedException | Αρχείο στο*path* περιέχει άνω και κάτω τελεία (:) στη μέση της συμβολοσειράς. |

### Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώρηση. Βλέπω[`ExtractToDirectory`](../extracttodirectory/) μέθοδος αποσυμπίεσης.

### Παραδείγματα

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### Δείτε επίσης

* class [SevenZipArchive](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchive/)
* συνέλευση [Aspose.Zip](../../../)


