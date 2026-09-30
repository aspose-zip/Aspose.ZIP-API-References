---
title: "LzmaArchiveSettings.LzmaArchiveSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor LzmaArchiveSettings. Menginisialisasi sebuah instance baru dari kelas LzmaArchiveSettings dengan ukuran kamus default sebesar 16 megabyte, jumlah byte cepat sebesar 32, dan bit konteks literal sebesar 3."
type: docs
weight: 10
url: /id/net/aspose.zip.lzma/lzmaarchivesettings/lzmaarchivesettings/
---
## LzmaArchiveSettings constructor

Menginisialisasi sebuah instance baru dari kelas [`LzmaArchiveSettings`](../) dengan ukuran kamus default sebesar 16 megabyte, jumlah byte cepat sebesar 32, dan bit konteks literal sebesar 3.

```csharp
public LzmaArchiveSettings()
```

## Contoh

```csharp
using (LzmaArchive archive = new LzmaArchive(new LzmaArchiveSettings() { DictionarySize = 1048576 })
{
    archive.SetSource("data.bin");
    archive.Save(lzmaFile);
}
```

### Lihat Juga

* class [LzmaArchiveSettings](../)
* namespace [Aspose.Zip.LZMA](../../lzmaarchivesettings/)
* assembly [Aspose.Zip](../../../)


