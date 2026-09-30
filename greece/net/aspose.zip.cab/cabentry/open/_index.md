---
title: "CabEntry.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος CabEntry. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα stream με το περιεχόμενο της καταχώρησης"
type: docs
weight: 50
url: /el/net/aspose.zip.cab/cabentry/open/
---
## CabEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης.

```csharp
public Stream Open()
```

### Τιμή Επιστροφής

Το stream που αντιπροσωπεύει τα περιεχόμενα της καταχώρησης.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| NotSupportedException | Η αρχικοποίηση του Stream απέτυχε λόγω λανθασμένων δεδομένων. |
| InvalidDataException | Το αρχείο είναι κατεστραμμένο. |
| InvalidOperationException | Η καταχώρηση ανήκει σε ένα αρχείο που έχει προετοιμαστεί για σύνθεση. |
| ObjectDisposedException | Εκτοπίζεται εάν η πηγή έχει διαγραφεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

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

* class [CabEntry](../)
* namespace [Aspose.Zip.Cab](../../cabentry/)
* assembly [Aspose.Zip](../../../)


