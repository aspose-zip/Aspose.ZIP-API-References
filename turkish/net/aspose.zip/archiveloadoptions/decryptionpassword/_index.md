---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP for .NET API Referansı
description: ArchiveLoadOptions mülk. Girişlerin şifresini çözmek için parolayı alır veya ayarlar.
type: docs
weight: 20
url: /tr/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Girişlerin şifresini çözmek için parolayı alır veya ayarlar.

```csharp
public string DecryptionPassword { get; set; }
```

### Örnekler

Arşiv çıkarma işleminde bir kez şifre çözme şifresi sağlayabilirsiniz.

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

### Ayrıca bakınız

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* ad alanı [Aspose.Zip](../../archiveloadoptions/)
* toplantı [Aspose.Zip](../../../)


