---
title: "ArchiveEntry.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος ArchiveEntry. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα stream με το αποσυμπιεσμένο περιεχόμενο της καταχώρησης"
type: docs
weight: 120
url: /el/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το αποσυμπιεσμένο περιεχόμενο της καταχώρησης.

```csharp
public Stream Open(string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Προαιρετικό password για αποκρυπτογράφηση. |

### Τιμή Επιστροφής

Το stream που αντιπροσωπεύει τα περιεχόμενα της καταχώρησης.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Το αρχείο βρίσκεται σε λανθασμένη κατάσταση. |
| ObjectDisposedException | Εκτοπίζεται εάν το αρχείο έχει διαγραφεί. |

## Παρατηρήσεις

Διαβάστε από το stream για να λάβετε το αρχικό περιεχόμενο ενός αρχείου. Δείτε την ενότητα παραδειγμάτων.

## Παραδείγματα

Χρήση:

```csharp
Stream decompressed = entry.Open();
```

.NET 4.0 και νεότερο - χρησιμοποιήστε τη μέθοδο Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 και παλαιότερο - αντιγράψτε τα bytes χειροκίνητα:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Δείτε επίσης

* class [ArchiveEntry](../)
* namespace [Aspose.Zip](../../archiveentry/)
* assembly [Aspose.Zip](../../../)


