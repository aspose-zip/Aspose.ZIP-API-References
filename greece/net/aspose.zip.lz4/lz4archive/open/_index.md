---
title: "Lz4Archive.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Lz4Archive μέθοδος. Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου"
type: docs
weight: 50
url: /el/net/aspose.zip.lz4/lz4archive/open/
---
## Lz4Archive.Open method

Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου.

```csharp
public Stream Open()
```

### Τιμή Επιστροφής

Η ροή που αντιπροσωπεύει το περιεχόμενο του αρχείου.

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| EndOfStreamException | Η πηγή ροής είναι πολύ μικρή. |
| InvalidDataException | Βρέθηκαν λανθασμένα bytes κατά την έναρξη αποκωδικοποίησης. |
| InvalidOperationException | Το αρχείο είναι προετοιμασμένο για σύνθεση. |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |
| IOException | Παρουσιάστηκε σφάλμα I/O. |

## Παρατηρήσεις

Διαβάστε από το stream για να λάβετε το αρχικό περιεχόμενο ενός αρχείου. Δείτε την ενότητα παραδειγμάτων.

## Παραδείγματα

Εξάγει το αρχείο και αντιγράφει το εξαγόμενο περιεχόμενο σε ροή αρχείου.

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
    using (var extracted = File.Create("data.bin"))
    {
        var unpacked = archive.Open();
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }            
}
```

Μπορείτε να χρησιμοποιήσετε τη μέθοδο Stream.CopyTo για .NET 4.0 και νεότερες εκδόσεις:

```csharp
unpacked.CopyTo(extracted);
```

### Δείτε επίσης

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


