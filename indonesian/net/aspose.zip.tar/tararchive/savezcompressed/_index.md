---
title: TarArchive.SaveZCompressed
second_title: Aspose.ZIP untuk Referensi .NET API
description: TarArchive metode. Menyimpan arsip ke aliran dengan kompresi Z.
type: docs
weight: 160
url: /id/net/aspose.zip.tar/tararchive/savezcompressed/
---
## SaveZCompressed(Stream, TarFormat?) {#savezcompressed}

Menyimpan arsip ke aliran dengan kompresi Z.

```csharp
public void SaveZCompressed(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, TarFormat?) {#savezcompressed_1}

Menyimpan arsip ke jalur demi jalur dengan kompresi Z.

```csharp
public void SaveZCompressed(string path, TarFormat? format = default)
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
        archive.SaveZCompressed("result.tar.Z");
    }
}
```

### Lihat juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* ruang nama [Aspose.Zip.Tar](../../tararchive/)
* perakitan [Aspose.Zip](../../../)


