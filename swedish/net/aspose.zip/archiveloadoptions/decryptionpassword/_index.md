---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP för .NET API-referens
description: ArchiveLoadOptions fast egendom. Hämtar eller ställer in lösenordet för att dekryptera poster.
type: docs
weight: 20
url: /sv/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Hämtar eller ställer in lösenordet för att dekryptera poster.

```csharp
public string DecryptionPassword { get; set; }
```

### Exempel

Du kan ange dekrypteringslösenord en gång vid arkivutvinning.

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

### Se även

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* namnutrymme [Aspose.Zip](../../archiveloadoptions/)
* hopsättning [Aspose.Zip](../../../)


