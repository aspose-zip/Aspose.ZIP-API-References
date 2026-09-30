---
title: "ArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα ArchiveLoadOptions. Λαμβάνει ή ορίζει την κωδικοποίηση για τα ονόματα των καταχωρήσεων"
type: docs
weight: 40
url: /el/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Λαμβάνει ή ορίζει την κωδικοποίηση για τα ονόματα των καταχωρίσεων.

```csharp
public Encoding Encoding { get; set; }
```

## Παραδείγματα

Το όνομα της καταχώρησης δημιουργείται χρησιμοποιώντας την καθορισμένη κωδικοποίηση ανεξάρτητα από τις ιδιότητες του αρχείου zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (var archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Δείτε επίσης

* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


