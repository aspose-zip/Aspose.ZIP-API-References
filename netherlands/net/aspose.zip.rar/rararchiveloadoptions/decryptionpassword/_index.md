---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP voor .NET API-referentie
description: RarArchiveLoadOptions eigendom. Haalt het wachtwoord op of stelt het in om items en itemnamen te decoderen.
type: docs
weight: 20
url: /nl/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Haalt het wachtwoord op of stelt het in om items en itemnamen te decoderen.

```csharp
public string DecryptionPassword { get; set; }
```

### Voorbeelden

U kunt het decoderingswachtwoord eenmaal opgeven bij het uitpakken van het archief.

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

### Zie ook

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* naamruimte [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* montage [Aspose.Zip](../../../)


