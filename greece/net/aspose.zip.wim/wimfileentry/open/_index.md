---
title: "WimFileEntry.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "WimFileEntry μέθοδος. Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης."
type: docs
weight: 30
url: /el/net/aspose.zip.wim/wimfileentry/open/
---
## WimFileEntry.Open method

Ανοίγει την καταχώρηση για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο της καταχώρησης.

```csharp
public Stream Open()
```

### Τιμή Επιστροφής

Το stream που αντιπροσωπεύει τα περιεχόμενα της καταχώρησης.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
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

* class [WimFileEntry](../)
* namespace [Aspose.Zip.Wim](../../wimfileentry/)
* assembly [Aspose.Zip](../../../)


