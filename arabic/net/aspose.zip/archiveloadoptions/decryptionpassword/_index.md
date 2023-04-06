---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveLoadOptions ملكية. الحصول على أو تعيين كلمة المرور لفك تشفير الإدخالات.
type: docs
weight: 20
url: /ar/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

الحصول على أو تعيين كلمة المرور لفك تشفير الإدخالات.

```csharp
public string DecryptionPassword { get; set; }
```

### أمثلة

يمكنك توفير كلمة مرور فك التشفير مرة واحدة عند استخراج الأرشيف.

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

### أنظر أيضا

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* مساحة الاسم [Aspose.Zip](../../archiveloadoptions/)
* المجسم [Aspose.Zip](../../../)


