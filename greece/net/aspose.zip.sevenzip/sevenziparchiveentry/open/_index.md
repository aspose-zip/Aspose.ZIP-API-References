---
title: SevenZipArchiveEntry.Open
second_title: Aspose.ZIP για Αναφορά API .NET
description: SevenZipArchiveEntry μέθοδος. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με περιεχόμενο καταχώρισης.
type: docs
weight: 90
url: /el/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με περιεχόμενο καταχώρισης.

```csharp
public Stream Open(string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. |

### Επιστρεφόμενη Αξία

Η ροή που αντιπροσωπεύει τα περιεχόμενα της καταχώρισης.

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| InvalidOperationException | Το αρχείο δεν ανοίγει για εξαγωγή. - ή - Αυτή η καταχώρηση είναι ένας κατάλογος. |
| InvalidDataException | Λάθος δεδομένα μέσα στην καταχώρηση. |

### Παρατηρήσεις

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα παραδειγμάτων.

### Παραδείγματα

Χρήση:

.NET 4.0 και νεότερη έκδοση - χρησιμοποιήστε τη μέθοδο Stream.CopyTo:

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 και παλαιότερες εκδόσεις - αντιγραφή byte με μη αυτόματο τρόπο:

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Δείτε επίσης

* class [SevenZipArchiveEntry](../)
* χώρος ονομάτων [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* συνέλευση [Aspose.Zip](../../../)


