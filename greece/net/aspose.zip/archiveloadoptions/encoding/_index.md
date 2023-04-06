---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveLoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει την κωδικοποίηση για τα ονόματα των καταχωρήσεων.
type: docs
weight: 30
url: /el/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Λαμβάνει ή ορίζει την κωδικοποίηση για τα ονόματα των καταχωρήσεων.

```csharp
public Encoding Encoding { get; set; }
```

### Παραδείγματα

Όνομα καταχώρισης που συντέθηκε με χρήση καθορισμένης κωδικοποίησης ανεξάρτητα από τις ιδιότητες του αρχείου zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Δείτε επίσης

* class [ArchiveLoadOptions](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveloadoptions/)
* συνέλευση [Aspose.Zip](../../../)


