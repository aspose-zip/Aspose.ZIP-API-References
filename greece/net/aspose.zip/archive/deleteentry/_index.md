---
title: Archive.DeleteEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: Archive μέθοδος. Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.
type: docs
weight: 60
url: /el/net/aspose.zip/archive/deleteentry/
---
## DeleteEntry(ArchiveEntry) {#deleteentry}

Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.

```csharp
public Archive DeleteEntry(ArchiveEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | ArchiveEntry | Η καταχώρηση προς κατάργηση από τη λίστα καταχωρήσεων. |

### Επιστρεφόμενη Αξία

Το αρχείο με την καταχώρηση διαγράφηκε.

### Παραδείγματα

Δείτε πώς μπορείτε να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

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
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο.

```csharp
public Archive DeleteEntry(int entryIndex)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entryIndex | Int32 | Το μηδενικό ευρετήριο της καταχώρισης προς κατάργηση. |

### Επιστρεφόμενη Αξία

Το αρχείο με την καταχώρηση διαγράφηκε.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *entryIndex* είναι μικρότερο από 0.-ή-*entryIndex* είναι ίσο ή μεγαλύτερο από`Συμμετοχές` μετρώ. |

### Παραδείγματα

```csharp
using (var archive = new TarArchive("two_files.zip"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.zip");
}
```

### Δείτε επίσης

* class [Archive](../)
* χώρος ονομάτων [Aspose.Zip](../../archive/)
* συνέλευση [Aspose.Zip](../../../)


