---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CpioArchive. Menyimpan arsip ke aliran dengan kompresi Z"
type: docs
weight: 130
url: /id/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Menyimpan arsip ke aliran dengan kompresi Z.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Menyimpan arsip ke jalur berdasarkan jalur dengan kompresi Z.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| cpioFormat | CpioFormat | Mendefinisikan format header cpio. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentNullException | *path* adalah `null`. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| IOException | Terjadi kesalahan I/O. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |

## Contoh

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Lihat Juga

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


