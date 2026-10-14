---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية AlzArchiveLoadOptions. تُحصل أو تُعيّن كلمة المرور لفك تشفير الإدخالات"
type: docs
weight: 30
url: /ar/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

يحصل أو يضبط كلمة المرور لفك تشفير الإدخالات.

```csharp
public string DecryptionPassword { get; set; }
```

## أمثلة

يمكنك توفير كلمة مرور فك التشفير مرة واحدة عند استخراج الأرشيف.

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

### انظر أيضًا

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


