---
title: "ArchiveEntry.ExtractionProgressed"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Συμβάν ArchiveEntry. Ενεργοποιείται όταν εξάγεται ένα τμήμα της ακατέργαστης ροής"
type: docs
weight: 100
url: /el/net/aspose.zip/archiveentry/extractionprogressed/
---
## ArchiveEntry.ExtractionProgressed event

Ενεργοποιείται όταν ένα τμήμα ακατέργαστης ροής εξάγεται.

```csharp
public event EventHandler<ProgressCancelEventArgs> ExtractionProgressed;
```

## Παρατηρήσεις

Ο αποστολέας του συμβάντος είναι ένα στιγμιότυπο [`ArchiveEntry`](../). Είναι δυνατόν να ακυρωθεί η εξαγωγή.

## Παραδείγματα

Σε αυτό το παράδειγμα, ο διαχειριστής συμβάντων χρησιμοποιείται για τον υπολογισμό του ποσοστού του επεξεργασμένου μεγέθους σε ποσοστά.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => {  int percent = (int)((100 * e.ProceededBytes) / ((ArchiveEntry)s).UncompressedSize); };
```

Σε αυτό το παράδειγμα, ο διαχειριστής συμβάντων χρησιμοποιείται για ακύρωση μετά την εξαγωγή των πρώτων εκατοντάδων MB της καταχώρησης.

```csharp
a.Entries[0].ExtractionProgressed += (s, e) => { if (e.ProceededBytes > 100000000) e.Cancel = true; };
```

### Δείτε επίσης

* class [ProgressCancelEventArgs](../../progresscanceleventargs/)
* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


