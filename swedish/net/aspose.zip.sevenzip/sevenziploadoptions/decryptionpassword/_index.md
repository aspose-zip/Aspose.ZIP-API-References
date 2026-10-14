---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP för .NET API-referens"
description: "SevenZipLoadOptions-egenskap. Hämtar eller anger lösenordet för att dekryptera poster och postnamn"
type: docs
weight: 30
url: /sv/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Hämtar eller anger lösenordet för att dekryptera poster och postnamn.

```csharp
public string DecryptionPassword { get; set; }
```

## Exempel

Du kan ange dekrypteringslösenordet en gång vid arkivextraktion.

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

### Se även

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


