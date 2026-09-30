---
title: "GzipArchive.Open"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "GzipArchive μέθοδος. Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με το περιεχόμενο του αρχείου"
type: docs
weight: 70
url: /el/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

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

Διαβάστε από το stream για να λάβετε το αρχικό περιεχόμενο ενός αρχείου. Δείτε την ενότητα παραδειγμάτων.

## Παραδείγματα

Εξάγει το αρχείο και αντιγράφει το εξαγόμενο περιεχόμενο σε ροή αρχείου.

```csharp
using (var archive = new GzipArchive("archive.gz"))
{
    using (var extracted = File.Create("data.bin"))
    {
        using(var unpacked = archive.Open())
        {
            byte[] b = new byte[8192];
            int bytesRead;
            while (0 < (bytesRead = unpacked.Read(b, 0, b.Length)))
                extracted.Write(b, 0, bytesRead);
        }
    }            
}
```

Μπορείτε να χρησιμοποιήσετε τη μέθοδο Stream.CopyTo για .NET 4.0 και νεότερες εκδόσεις:

```csharp
unpacked.CopyTo(extracted);
```

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


