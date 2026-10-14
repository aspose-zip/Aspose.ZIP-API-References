---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "SevenZipLoadOptions özelliği. Girdileri ve giriş adlarını çözmek için şifreyi alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Girişleri ve giriş adlarını çözmek için şifreyi alır veya ayarlar.

```csharp
public string DecryptionPassword { get; set; }
```

## Örnekler

Arşiv çıkarma sırasında bir kez şifre sağlayabilirsiniz.

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

### Ayrıca Bakınız

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


