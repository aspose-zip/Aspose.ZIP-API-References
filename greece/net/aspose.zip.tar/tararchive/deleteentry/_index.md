---
title: "TarArchive.DeleteEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος TarArchive. Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων"
type: docs
weight: 120
url: /el/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| καταχώρηση | TarEntry | Η καταχώρηση που θα αφαιρεθεί από τη λίστα καταχωρήσεων. |

### Τιμή Επιστροφής

Το αρχείο με τη διαγραμμένη καταχώρηση.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παραδείγματα

Ακολουθεί ο τρόπος για να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

```csharp
using (var archive = new TarArchive("archive.tar"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputTarFile);
}
```

### Δείτε επίσης

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
| ObjectDisposedException | Το αρχείο έχει απελευθερωθεί και δεν μπορεί να χρησιμοποιηθεί |

## Παραδείγματα

```csharp
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


