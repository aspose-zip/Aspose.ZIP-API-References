---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti SevenZipLoadOptions. Mendapatkan atau mengatur password untuk mendekripsi entri dan nama entri"
type: docs
weight: 30
url: /id/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Mendapatkan atau mengatur kata sandi untuk mendekripsi entri dan nama entri.

```csharp
public string DecryptionPassword { get; set; }
```

## Contoh

Anda dapat memberikan kata sandi dekripsi satu kali saat ekstraksi arsip.

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

### Lihat Juga

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


