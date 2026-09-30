---
title: "SevenZipArchiveEntry.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SevenZipArchiveEntry μέθοδος. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης"
type: docs
weight: 90
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης.

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
| InvalidOperationException | Το αρχείο δεν είναι ανοικτό για εξαγωγή. - ή - Αυτή η καταχώρηση είναι κατάλογος. |
| InvalidDataException | Λάθος δεδομένα μέσα στην καταχώρηση. |
| ObjectDisposedException | Εκτοπίζεται εάν η ροή πηγής έχει διαγραφεί. |

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

* class [SevenZipArchiveEntry](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* assembly [Aspose.Zip](../../../)


