---
title: "UueArchive.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "UueArchive μέθοδος. Ανοίγει το αρχείο για αποκωδικοποίηση και παρέχει μια ροή με το περιεχόμενο του αρχείου"
type: docs
weight: 60
url: /el/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Ανοίγει το αρχείο για αποκωδικοποίηση και παρέχει μια ροή με το περιεχόμενο του αρχείου.

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

Διαβάστε από το stream για να λάβετε το αρχικό περιεχόμενο ενός αρχείου. Δείτε την ενότητα παραδειγμάτων.

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

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


