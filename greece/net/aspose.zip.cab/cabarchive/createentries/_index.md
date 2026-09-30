---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος CabArchive. Προσθέτει στο αρχείο όλα τα αρχεία αναδρομικά από τον καθορισμένο φάκελο."
type: docs
weight: 30
url: /el/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Προσθέτει στο αρχείο όλα τα αρχεία, αναδρομικά, από τον καθορισμένο φάκελο.

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| directory | DirectoryInfo | Φάκελος προς συμπίεση. |
| includeRootDirectory | Boolean | Δείχνει αν θα συμπεριληφθεί το όνομα του ριζικού φακέλου στις διαδρομές των καταχωρήσεων. |

### Τιμή Επιστροφής

Το τρέχον παράδειγμα [`CabArchive`](../).

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *directory* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| DirectoryNotFoundException | *directory* δεν μπορεί να βρεθεί. |
| SecurityException | Ο καλών δεν διαθέτει την απαιτούμενη άδεια για πρόσβαση στο *directory* ή στο περιεχόμενό του. |
| UnauthorizedAccessException | Η πρόσβαση στο *directory* ή σε ένα από τα αρχεία του απορρίπτεται. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά την πρόσβαση στο *directory*. |
| PathTooLongException | Μια δημιουργημένη διαδρομή καταχώρησης υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή και δεν μπορεί να προσθέσει καταχωρήσεις. |

## Παραδείγματα

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### Δείτε επίσης

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Προσθέτει στο αρχείο όλα τα αρχεία αναδρομικά από τη διαδρομή του καθορισμένου φακέλου.

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceDirectory | String | Διαδρομή φακέλου για συμπίεση. |
| includeRootDirectory | Boolean | Δείχνει αν θα συμπεριληφθεί το όνομα του ριζικού φακέλου στις διαδρομές των καταχωρήσεων. |

### Τιμή Επιστροφής

Το τρέχον παράδειγμα [`CabArchive`](../).

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| ArgumentNullException | *sourceDirectory* είναι null. |
| DirectoryNotFoundException | *sourceDirectory* δεν μπορεί να βρεθεί. |
| SecurityException | Ο καλούν δεν διαθέτει την απαιτούμενη άδεια για πρόσβαση στο *sourceDirectory*. |
| UnauthorizedAccessException | Η πρόσβαση στο *sourceDirectory* απορρίπτεται. |
| PathTooLongException | Ο καθορισμένος *sourceDirectory* υπερβαίνει το μέγιστο μήκος που ορίζεται από το σύστημα. |
| ArgumentException | *sourceDirectory* είναι κενό, περιέχει μόνο κενά διαστήματα ή περιέχει μη έγκυρους χαρακτήρες. |
| IOException | Παρουσιάστηκε σφάλμα I/O κατά την πρόσβαση στο *sourceDirectory*. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για εξαγωγή και δεν μπορεί να προσθέσει καταχωρήσεις. |

## Παραδείγματα

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### Δείτε επίσης

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


