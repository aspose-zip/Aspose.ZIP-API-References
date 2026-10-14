---
title: "Bzip2Archive.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος Bzip2Archive. Ανοίγει το αρχείο για εξαγωγή και παρέχει ένα ρεύμα με το περιεχόμενο του αρχείου."
type: docs
weight: 50
url: /el/net/aspose.zip.bzip2/bzip2archive/open/
---
## Bzip2Archive.Open method

Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου.

```csharp
public Stream Open()
```

### Τιμή Επιστροφής

Η ροή που αντιπροσωπεύει το περιεχόμενο του αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Διαβάστε από το ρεύμα για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα παραδειγμάτων.

## Παραδείγματα

Χρήση:

```csharp
Stream decompressed = archive.Open();
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

* class [Bzip2Archive](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2archive/)
* assembly [Aspose.Zip](../../../)


