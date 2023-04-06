---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP για Αναφορά API .NET
description: ArchiveLoadOptions ιδιοκτησία. Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των εγγραφών.
type: docs
weight: 20
url: /el/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των εγγραφών.

```csharp
public string DecryptionPassword { get; set; }
```

### Παραδείγματα

Μπορείτε να δώσετε κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή αρχείου.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.zip"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* χώρος ονομάτων [Aspose.Zip](../../archiveloadoptions/)
* συνέλευση [Aspose.Zip](../../../)


