---
title: TarArchive.SaveGzipped
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive metode. Menyimpan arsip ke aliran dengan kompresi gzip.
type: docs
weight: 130
url: /id/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Menyimpan arsip ke aliran dengan kompresi gzip.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| format | Nullable`1 | Mendefinisikan format tajuk tar. Nilai null akan diperlakukan sebagai UStar jika memungkinkan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah nol. |
| ArgumentException | *output* tidak dapat ditulis. |

### Perkataan

*output*harus dapat ditulis.

### Contoh

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Lihat juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Menyimpan arsip ke file dengan jalur dengan kompresi gzip.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |
| format | Nullable`1 | Mendefinisikan format tajuk tar. Nilai null akan diperlakukan sebagai UStar jika memungkinkan. |

### Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### Lihat juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


