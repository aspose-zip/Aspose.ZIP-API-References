---
title: ArchiveLoadOptions.Encoding
second_title: Aspose.ZIP untuk Referensi .NET API
description: ArchiveLoadOptions Properti. Mendapat atau mengatur pengkodean untuk nama entri.
type: docs
weight: 30
url: /id/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Mendapat atau mengatur pengkodean untuk nama entri.

```csharp
public Encoding Encoding { get; set; }
```

### Contoh

Nama entri disusun menggunakan pengkodean yang ditentukan terlepas dari properti file zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Lihat juga

* class [ArchiveLoadOptions](../)
* ruang nama [Aspose.Zip](../../archiveloadoptions/)
* perakitan [Aspose.Zip](../../../)


