---
title: "Archive.DeleteEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Archive. Αφαιρεί την πρώτη εμφάνιση της συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων."
type: docs
weight: 70
url: /el/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Αφαιρεί την πρώτη εμφάνιση της συγκεκριμένης καταχώρησης από τη λίστα καταχωρίσεων.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| καταχώρηση | ArchiveEntry | Η καταχώρηση που θα αφαιρεθεί από τη λίστα καταχωρήσεων. |

### Τιμή Επιστροφής

Το αρχείο με τη διαγραμμένη καταχώρηση.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί. |
| InvalidOperationException | Εκτοξεύεται όταν η διαγραφή της καταχώρησης δεν είναι έγκυρη λόγω της τρέχουσας κατάστασης του αρχείου. |

## Παραδείγματα

Ακολουθεί ο τρόπος για να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

```csharp
using (var archive = new Archive("archive.zip"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save("last_entry.zip");
}
```

### Δείτε επίσης

* class [ArchiveEntry](../../archiveentry/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entryIndex | Int32 | Ο μηδενικός δείκτης της καταχώρησης που θα αφαιρεθεί. |

### Τιμή Επιστροφής

Το αρχείο με τη διαγραμμένη καταχώρηση.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το Archive έχει διαγραφεί. |
| ArgumentOutOfRangeException | *entryIndex* είναι μικρότερο του 0.-ή- *entryIndex* είναι ίσο ή μεγαλύτερο από τον αριθμό των `Entries` count. |
| InvalidOperationException | Εκτοξεύεται όταν η διαγραφή της καταχώρησης δεν είναι έγκυρη λόγω της τρέχουσας κατάστασης του αρχείου. |

## Παραδείγματα

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Δείτε επίσης

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


