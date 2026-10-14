---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AlzArchiveLoadOptions eigenschap. Haalt het wachtwoord op of stelt het in om items te ontsleutelen"
type: docs
weight: 30
url: /nl/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Haalt het wachtwoord op of stelt het in om items te ontsleutelen.

```csharp
public string DecryptionPassword { get; set; }
```

## Voorbeelden

U kunt het ontsleutelingswachtwoord één keer opgeven bij het uitpakken van het archief.

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

### Zie ook

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


