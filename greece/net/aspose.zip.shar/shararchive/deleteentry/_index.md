---
title: SharArchive.DeleteEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: SharArchive μέθοδος. Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.
type: docs
weight: 50
url: /el/net/aspose.zip.shar/shararchive/deleteentry/
---
## DeleteEntry(SharEntry) {#deleteentry}

Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.

```csharp
public SharArchive DeleteEntry(SharEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | SharEntry | Η καταχώρηση προς κατάργηση από τη λίστα καταχωρήσεων. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Shar.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *entry* είναι μηδενικό. |

### Παραδείγματα

Δείτε πώς μπορείτε να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

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
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο.

```csharp
public SharArchive DeleteEntry(int entryIndex)
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
using (var archive = new SharArchive("two_files.shar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.shar");
}
```

### Δείτε επίσης

* class [SharArchive](../)
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)


