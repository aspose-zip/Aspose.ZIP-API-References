---
title: CpioArchive.DeleteEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive μέθοδος. Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.
type: docs
weight: 50
url: /el/net/aspose.zip.cpio/cpioarchive/deleteentry/
---
## DeleteEntry(CpioEntry) {#deleteentry}

Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.

```csharp
public CpioArchive DeleteEntry(CpioEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | CpioEntry | Η καταχώρηση προς κατάργηση από τη λίστα καταχωρήσεων. |

### Επιστρεφόμενη Αξία

Περίπτωση εισαγωγής Cpio.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *entry* είναι μηδενικό. |

### Παραδείγματα

Δείτε πώς μπορείτε να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

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
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο.

```csharp
public CpioArchive DeleteEntry(int entryIndex)
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
using (var archive = new CpioArchive("two_files.cpio"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.cpio");
}
```

### Δείτε επίσης

* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


