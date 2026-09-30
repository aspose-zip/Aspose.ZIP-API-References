---
title: "AppleArchive.AppleArchive"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "AppleArchive constructor. Αρχικοποιεί μια νέα παρουσία της κλάσης AppleArchive με ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις"
type: docs
weight: 10
url: /el/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`AppleArchive`](../) με ρυθμίσεις που χρησιμοποιούνται για τις συντεθειμένες καταχωρίσεις.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Ρυθμίσεις που χρησιμοποιούνται κατά τη σύνθεση ενός νέου Apple Archive. |

### Δείτε επίσης

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`AppleArchive`](../) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sourceStream | Stream | Η πηγή του αρχείου. |
| loadOptions | AppleArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *sourceStream* είναι null. |
| ArgumentException | *sourceStream* δεν είναι δυνατόν να γίνει αναζήτηση. |
| InvalidDataException | *sourceStream* δεν είναι έγκυρο Apple Archive. |
| EndOfStreamException | Η ροή τερματίζει απροσδόκητα κατά την ανάλυση των καταχωρίσεων του αρχείου. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τις μεθόδους [`ExtractToDirectory`](../extracttodirectory/) και [`Open`](../../applearchiveentry/open/) για αποσυμπίεση.

### Δείτε επίσης

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`AppleArchive`](../) και συνθέτει μια λίστα καταχωρίσεων που μπορεί να εξαχθεί από το αρχείο.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | String | Η πλήρης ή σχετική διαδρομή προς το αρχείο του αρχείου. |
| loadOptions | AppleArchiveLoadOptions | Επιλογές για τη φόρτωση υπάρχοντος αρχείου. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentNullException | *path* είναι null. |
| FileNotFoundException | Το αρχείο δεν βρέθηκε. |
| InvalidDataException | *path* δεν είναι έγκυρο Apple Archive. |
| EndOfStreamException | Η ροή τερματίζει απροσδόκητα κατά την ανάλυση των καταχωρίσεων του αρχείου. |

## Παρατηρήσεις

Αυτός ο κατασκευαστής δεν αποσυμπιέζει καμία καταχώριση. Δείτε τις μεθόδους [`ExtractToDirectory`](../extracttodirectory/) και [`Open`](../../applearchiveentry/open/) για αποσυμπίεση.

### Δείτε επίσης

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


