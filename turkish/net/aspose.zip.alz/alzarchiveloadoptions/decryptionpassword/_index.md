---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "AlzArchiveLoadOptions özelliği. Girişleri çözmek için şifreyi alır veya ayarlar."
type: docs
weight: 30
url: /tr/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Girişleri şifre çözmek için parolayı alır veya ayarlar.

```csharp
public string DecryptionPassword { get; set; }
```

## Örnekler

Arşiv çıkarma sırasında bir kez şifre sağlayabilirsiniz.

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

### Ayrıca Bakınız

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


