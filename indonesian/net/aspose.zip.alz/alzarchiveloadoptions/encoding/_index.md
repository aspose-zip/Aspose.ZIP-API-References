---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti AlzArchiveLoadOptions. Mendapatkan atau mengatur encoding untuk nama entri. Defaultnya adalah kode halaman Windows Korea 949 CP949."
type: docs
weight: 40
url: /id/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Mendapatkan atau mengatur pengkodean untuk nama entri. Default adalah kode halaman Windows Korea 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Catatan

Arsip ALZ secara historis menyimpan nama file menggunakan kode halaman ANSI Windows Korea.

## Contoh

Nama entri disusun menggunakan encoding yang ditentukan.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Lihat Juga

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


