---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα AlzArchiveLoadOptions. Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων."
type: docs
weight: 30
url: /el/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρίσεων.

```csharp
public string DecryptionPassword { get; set; }
```

## Παραδείγματα

Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.alz"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
        {
            using (var decompressed = archive.Entries[0].Open())
            {
                byte[] b = new byte[8192];
                int bytesRead;
                while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
                    extracted.Write(b, 0, bytesRead);
                
            }
        }
    }
}
```

### Δείτε επίσης

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


