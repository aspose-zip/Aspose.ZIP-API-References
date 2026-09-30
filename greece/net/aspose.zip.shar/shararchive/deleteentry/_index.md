---
title: "SharArchive.DeleteEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SharArchive method. Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων"
type: docs
weight: 50
url: /el/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| καταχώρηση | SharEntry | Η καταχώρηση που θα αφαιρεθεί από τη λίστα καταχωρήσεων. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Shar.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *entry* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι ανοιχτό για εξαγωγή. |

## Παραδείγματα

Ακολουθεί ο τρόπος για να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

```csharp
using (var archive = new SharArchive("archive.shar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputSharFile);
}
```

### Δείτε επίσης

* class [SharEntry](../../sharentry/)
* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη.

```csharp
public SharArchive DeleteEntry(int entryIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entryIndex | Int32 | Ο μηδενικός δείκτης της καταχώρησης που θα αφαιρεθεί. |

### Τιμή Επιστροφής

Το αρχείο με τη διαγραμμένη καταχώρηση.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* είναι μικρότερο του 0.-ή- *entryIndex* είναι ίσο ή μεγαλύτερο από τον αριθμό των `Entries` count. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| InvalidOperationException | Αυτό το αρχείο είναι ανοιχτό για εξαγωγή. |

## Παραδείγματα

```csharp
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Δείτε επίσης

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


