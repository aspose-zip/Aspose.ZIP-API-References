---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "SevenZipLoadOptions-eigenschap. Haalt het wachtwoord op of stelt het in om items en itemnamen te ontsleutelen"
type: docs
weight: 30
url: /nl/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Haalt het wachtwoord op of stelt het in om items en itemnamen te ontsleutelen.

```csharp
public string DecryptionPassword { get; set; }
```

## Voorbeelden

U kunt het ontsleutelingswachtwoord één keer opgeven bij het uitpakken van het archief.

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

### Zie ook

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


