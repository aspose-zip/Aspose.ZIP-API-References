---
title: TarArchive.SaveXzCompressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive metode. Menyimpan arsip ke aliran dengan kompresi xz.
type: docs
weight: 150
url: /id/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Menyimpan arsip ke aliran dengan kompresi xz.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| format | Nullable`1 | Mendefinisikan format tajuk tar. Nilai null akan diperlakukan sebagai UStar jika memungkinkan. |
| settings | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, jenis cek. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah nol. |
| ArgumentException | *output* tidak dapat ditulis. |

### Perkataan

*output*Aliran harus dapat ditulisi.

### Contoh

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Lihat juga

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Menyimpan arsip ke jalur demi jalur dengan kompresi xz.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |
| format | Nullable`1 | Mendefinisikan format tajuk tar. Nilai null akan diperlakukan sebagai UStar jika memungkinkan. |
| settings | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, jenis cek. |

### Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Lihat juga

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


