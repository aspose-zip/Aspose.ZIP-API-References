---
title: TarArchive.DeleteEntry
second_title: Aspose.ZIP για Αναφορά API .NET
description: TarArchive μέθοδος. Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.
type: docs
weight: 90
url: /el/net/aspose.zip.tar/tararchive/deleteentry/
---
## DeleteEntry(TarEntry) {#deleteentry}

Καταργεί την πρώτη εμφάνιση μιας συγκεκριμένης καταχώρισης από τη λίστα καταχωρήσεων.

```csharp
public TarArchive DeleteEntry(TarEntry entry)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| entry | TarEntry | Η καταχώρηση προς κατάργηση από τη λίστα καταχωρήσεων. |

### Επιστρεφόμενη Αξία

Το αρχείο με την καταχώρηση διαγράφηκε.

### Παραδείγματα

Δείτε πώς μπορείτε να αφαιρέσετε όλες τις καταχωρήσεις εκτός από την τελευταία:

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
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## DeleteEntry(int) {#deleteentry_1}

Αφαιρεί την καταχώρηση από τη λίστα καταχωρήσεων κατά ευρετήριο.

```csharp
public TarArchive DeleteEntry(int entryIndex)
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
using (var archive = new TarArchive("two_files.tar"))
{
    archive.DeleteEntry(0);
    archive.Save("single_file.tar");
}
```

### Δείτε επίσης

* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)


