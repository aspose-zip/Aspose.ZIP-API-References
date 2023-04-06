---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP لمرجع .NET API
description: RarArchiveLoadOptions ملكية. الحصول على أو تعيين كلمة المرور لفك تشفير الإدخالات وأسماء الإدخال.
type: docs
weight: 20
url: /ar/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

الحصول على أو تعيين كلمة المرور لفك تشفير الإدخالات وأسماء الإدخال.

```csharp
public string DecryptionPassword { get; set; }
```

### أمثلة

يمكنك توفير كلمة مرور فك التشفير مرة واحدة عند استخراج الأرشيف.

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

### أنظر أيضا

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* مساحة الاسم [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* المجسم [Aspose.Zip](../../../)


