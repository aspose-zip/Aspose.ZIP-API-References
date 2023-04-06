---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP för .NET API-referens
description: RarArchiveLoadOptions fast egendom. Hämtar eller ställer in lösenordet för att dekryptera poster och namn på poster.
type: docs
weight: 20
url: /sv/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Hämtar eller ställer in lösenordet för att dekryptera poster och namn på poster.

```csharp
public string DecryptionPassword { get; set; }
```

### Exempel

Du kan ange dekrypteringslösenord en gång vid arkivutvinning.

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

### Se även

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* namnutrymme [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* hopsättning [Aspose.Zip](../../../)


