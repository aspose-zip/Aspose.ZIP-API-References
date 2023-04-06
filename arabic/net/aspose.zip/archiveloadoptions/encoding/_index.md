---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP لمرجع .NET API
description: ArchiveLoadOptions ملكية. الحصول على أو تعيين ترميز أسماء الإدخالات.
type: docs
weight: 30
url: /ar/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

الحصول على أو تعيين ترميز أسماء الإدخالات.

```csharp
public Encoding Encoding { get; set; }
```

### أمثلة

يتكون اسم الإدخال باستخدام ترميز محدد بغض النظر عن خصائص الملف المضغوط.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### أنظر أيضا

* class [ArchiveLoadOptions](../)
* مساحة الاسم [Aspose.Zip](../../archiveloadoptions/)
* المجسم [Aspose.Zip](../../../)


