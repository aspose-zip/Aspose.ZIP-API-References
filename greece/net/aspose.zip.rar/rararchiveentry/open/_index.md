---
title: "RarArchiveEntry.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "RarArchiveEntry μέθοδος. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ροή με αποσυμπιεσμένο περιεχόμενο της καταχώρησης."
type: docs
weight: 100
url: /el/net/aspose.zip.rar/rararchiveentry/open/
---
## RarArchiveEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει μια ροή με το αποσυμπιεσμένο περιεχόμενο της καταχώρησης.

```csharp
public Stream Open(string password = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| password | String | Προαιρετικός κωδικός πρόσβασης για αποκρυπτογράφηση. Μπορεί επίσης να οριστεί μέσα στο [`DecryptionPassword`](../../rararchiveloadoptions/decryptionpassword/). |

### Τιμή Επιστροφής

Το stream που αντιπροσωπεύει τα περιεχόμενα της καταχώρησης.

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

* class [RarArchiveEntry](../)
* namespace [Aspose.Zip.Rar](../../rararchiveentry/)
* assembly [Aspose.Zip](../../../)


