---
title: GzipArchive.Open
second_title: Aspose.ZIP για Αναφορά API .NET
description: GzipArchive μέθοδος. Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με περιεχόμενο αρχειοθέτησης.
type: docs
weight: 50
url: /el/net/aspose.zip.gzip/gziparchive/open/
---
## GzipArchive.Open method

Ανοίγει το αρχείο για εξαγωγή και παρέχει μια ροή με περιεχόμενο αρχειοθέτησης.

```csharp
public Stream Open()
```

### Επιστρεφόμενη Αξία

Η ροή που αντιπροσωπεύει τα περιεχόμενα του αρχείου.

### Παρατηρήσεις

Διαβάστε από τη ροή για να λάβετε το αρχικό περιεχόμενο του αρχείου. Δείτε την ενότητα παραδειγμάτων.

### Παραδείγματα

Εξάγει το αρχείο και αντιγράφει το εξαγόμενο περιεχόμενο στη ροή αρχείων.

Μπορείτε να χρησιμοποιήσετε τη μέθοδο Stream.CopyTo για .NET 4.0 και νεότερη έκδοση:

```csharp
unpacked.CopyTo(extracted);
```

```csharp
using (var archive = new GzipArchive("archive.gz"))
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

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)


