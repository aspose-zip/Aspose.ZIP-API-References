---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "SevenZipLoadOptions ιδιότητα. Παίρνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση καταχωρήσεων και ονομάτων καταχωρήσεων"
type: docs
weight: 30
url: /el/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Λαμβάνει ή ορίζει τον κωδικό πρόσβασης για την αποκρυπτογράφηση των καταχωρήσεων και των ονομάτων καταχωρήσεων.

```csharp
public string DecryptionPassword { get; set; }
```

## Παραδείγματα

Μπορείτε να παρέχετε τον κωδικό αποκρυπτογράφησης μία φορά κατά την εξαγωγή του αρχείου.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


