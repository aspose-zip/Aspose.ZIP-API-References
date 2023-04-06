---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: CpioArchive metode. Menyimpan arsip ke aliran dengan kompresi xz.
type: docs
weight: 100
url: /id/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Menyimpan arsip ke aliran dengan kompresi xz.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| cpioFormat | CpioFormat | Mendefinisikan format tajuk cpio. |
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
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Lihat juga

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Menyimpan arsip ke jalur demi jalur dengan kompresi xz.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan menunjuk ke file yang sudah ada, itu akan ditimpa. |
| cpioFormat | CpioFormat | Mendefinisikan format tajuk cpio. |
| settings | XzArchiveSettings | Kumpulan pengaturan arsip xz tertentu: ukuran kamus, ukuran blok, jenis cek. |

### Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### Lihat juga

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* ruang nama [Aspose.Zip.Cpio](../../cpioarchive/)
* perakitan [Aspose.Zip](../../../)


