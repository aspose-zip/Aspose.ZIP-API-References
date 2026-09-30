---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية SevenZipLoadOptions. يحصل أو يحدد كلمة المرور لفك تشفير الإدخالات وأسماء الإدخالات"
type: docs
weight: 30
url: /ar/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

يحصل على أو يضبط كلمة المرور لفك تشفير الإدخالات وأسماء الإدخالات.

```csharp
public string DecryptionPassword { get; set; }
```

## أمثلة

يمكنك توفير كلمة مرور فك التشفير مرة واحدة عند استخراج الأرشيف.

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

### انظر أيضًا

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


