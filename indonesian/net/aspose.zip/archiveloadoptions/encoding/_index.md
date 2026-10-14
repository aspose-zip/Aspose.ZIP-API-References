---
title: "ArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti ArchiveLoadOptions. Mendapatkan atau mengatur encoding untuk nama entri"
type: docs
weight: 40
url: /id/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

Mendapatkan atau mengatur pengkodean untuk nama entri.

```csharp
public Encoding Encoding { get; set; }
```

## Contoh

Nama entri disusun menggunakan encoding yang ditentukan terlepas dari properti file zip.

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (var archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### Lihat Juga

* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


