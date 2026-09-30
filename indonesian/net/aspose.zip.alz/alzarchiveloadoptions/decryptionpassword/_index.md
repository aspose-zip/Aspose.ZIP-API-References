---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti AlzArchiveLoadOptions. Mendapatkan atau mengatur kata sandi untuk mendekripsi entri."
type: docs
weight: 30
url: /id/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Mendapatkan atau mengatur kata sandi untuk mendekripsi entri.

```csharp
public string DecryptionPassword { get; set; }
```

## Contoh

Anda dapat memberikan kata sandi dekripsi satu kali saat ekstraksi arsip.

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

### Lihat Juga

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


