---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα AlzArchiveLoadOptions. Λαμβάνει ή ορίζει την κωδικοποίηση για τα ονόματα των καταχωρίσεων. Η προεπιλογή είναι η κορεατική κωδική σελίδα Windows 949 CP949."
type: docs
weight: 40
url: /el/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Λαμβάνει ή ορίζει την κωδικοποίηση για τα ονόματα των καταχωρήσεων. Η προεπιλογή είναι η κορεατική κωδική σελίδα Windows 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Παρατηρήσεις

Τα αρχεία ALZ ιστορικά αποθηκεύουν τα ονόματα αρχείων χρησιμοποιώντας την κορεατική κωδική σελίδα ANSI των Windows.

## Παραδείγματα

Το όνομα της καταχώρισης συντίθεται χρησιμοποιώντας την καθορισμένη κωδικοποίηση.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Δείτε επίσης

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


