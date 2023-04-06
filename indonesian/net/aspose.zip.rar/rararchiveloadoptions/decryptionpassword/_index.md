---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP untuk Referensi .NET API
description: RarArchiveLoadOptions Properti. Mendapatkan atau menyetel kata sandi untuk mendekripsi entri dan nama entri.
type: docs
weight: 20
url: /id/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Mendapatkan atau menyetel kata sandi untuk mendekripsi entri dan nama entri.

```csharp
public string DecryptionPassword { get; set; }
```

### Contoh

Anda dapat memberikan kata sandi dekripsi satu kali pada ekstraksi arsip.

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

### Lihat juga

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* ruang nama [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* perakitan [Aspose.Zip](../../../)


