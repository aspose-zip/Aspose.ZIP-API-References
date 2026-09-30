---
title: "CpioArchive.SaveZstandard"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CpioArchive. Menyimpan arsip ke aliran dengan kompresi Zstandard"
type: docs
weight: 140
url: /id/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Menyimpan arsip ke aliran dengan kompresi Zstandard.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| cpioFormat | CpioFormat | Mendefinisikan format header cpio. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *output* adalah null. |
| ArgumentException | *output* tidak dapat ditulis. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Catatan

*output* must be writable.

## Contoh

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
        }
    }
}
```

### Lihat Juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Menyimpan arsip ke file berdasarkan jalur dengan kompresi Zstandard.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| cpioFormat | CpioFormat | Mendefinisikan format header cpio. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *path* adalah string dengan panjang nol, hanya berisi spasi, atau berisi satu atau lebih karakter tidak valid sebagaimana didefinisikan oleh InvalidPathChars. |
| ArgumentNullException | *path* adalah `null`. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| IOException | Terjadi kesalahan I/O. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| UnauthorizedAccessException | Pemanggil tidak memiliki izin yang diperlukan. -atau- *path* menunjukkan file atau direktori hanya-baca. |

## Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Lihat Juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


