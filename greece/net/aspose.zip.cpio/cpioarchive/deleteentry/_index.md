---
title: "CpioArchive.DeleteEntry"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "CpioArchive μέθοδος. Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων"
type: docs
weight: 50
url: /el/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Αφαιρεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρησης από τη λίστα καταχωρήσεων.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| καταχώρηση | CpioEntry | Η καταχώρηση που θα αφαιρεθεί από τη λίστα καταχωρήσεων. |

### Τιμή Επιστροφής

Παράδειγμα καταχώρησης Cpio.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *entry* είναι null. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παραδείγματα

Ακολουθεί ο τρόπος για να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

```csharp
using (var archive = new CpioArchive("archive.cpio"))
{
    while (archive.Entries.Count > 1)
        archive.DeleteEntry(archive.Entries[0]);
    archive.Save(outputCpioFile);
}
```

### Δείτε επίσης

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρίσεων με βάση το δείκτη.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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

## Παραδείγματα

```csharp
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


