---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveLoadOptions Properti. Mendapat atau menyetel kata sandi untuk mendekripsi entri.
type: docs
weight: 20
url: /id/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Mendapat atau menyetel kata sandi untuk mendekripsi entri.

```csharp
public string DecryptionPassword { get; set; }
```

### Contoh

Anda dapat memberikan kata sandi dekripsi satu kali pada ekstraksi arsip.

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

### Lihat juga

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* ruang nama [Aspose.Zip](../../archiveloadoptions/)
* perakitan [Aspose.Zip](../../../)


