---
title: "RarArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα RarArchiveLoadOptions. Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρήσεων και των ονομάτων τους"
type: docs
weight: 30
url: /el/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρήσεων και των ονομάτων καταχωρήσεων.

```csharp
public string DecryptionPassword { get; set; }
```

## Παραδείγματα

Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.rar"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (RarArchive archive = new RarArchive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* namespace [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


