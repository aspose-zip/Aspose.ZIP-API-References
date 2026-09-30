---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AlzArchiveLoadOptions-egenskap. Hämtar eller anger lösenordet för att dekryptera poster."
type: docs
weight: 30
url: /sv/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Hämtar eller anger lösenordet för att dekryptera poster.

```csharp
public string DecryptionPassword { get; set; }
```

## Exempel

Du kan ange dekrypteringslösenordet en gång vid arkivextraktion.

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

### Se även

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


