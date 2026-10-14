---
title: "TarArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Menyimpan arsip ke aliran yang disediakan"
type: docs
weight: 150
url: /id/net/aspose.zip.tar/tararchive/save/
---
## Save(Stream, TarFormat?) {#save}

Menyimpan arsip ke aliran yang disediakan.

```csharp
public void Save(Stream output, TarFormat? format = default)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| output | Stream | Aliran tujuan. |
| format | Nullable`1 | Mendefinisikan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *output* tidak dapat ditulis. - or - *output* adalah aliran yang sama dari mana kami mengekstrak. Arsip telah dibuang dan tidak dapat digunakan - OR - Tidak mungkin menyimpan arsip dalam *format* karena pembatasan format. |

## Catatan

*output* must be writable.

## Contoh

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry1", "data.bin");
        archive.Save(tarFile);
    }
}       
```

### Lihat Juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, TarFormat?) {#save_1}

Menyimpan arsip ke file tujuan yang disediakan.

```csharp
public void Save(string destinationFileName, TarFormat? format = default)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationFileName | String | Jalur arsip yang akan dibuat. Jika nama file yang ditentukan mengarah ke file yang sudah ada, file tersebut akan ditimpa. |
| format | Nullable`1 | Mendefinisikan format header tar. Nilai null akan diperlakukan sebagai USTar bila memungkinkan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *destinationFileName* adalah string dengan panjang nol, hanya berisi spasi putih, atau berisi satu atau lebih karakter tidak valid sebagaimana didefinisikan oleh System.IO.Path.InvalidPathChars. |
| ArgumentNullException | *destinationFileName* bernilai null. |
| PathTooLongException | *destinationFileName* yang ditentukan, nama file, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. |
| DirectoryNotFoundException | *destinationFileName* yang ditentukan tidak valid, (misalnya, berada pada drive yang tidak dipetakan). |
| IOException | Terjadi kesalahan I/O saat membuka file. |
| UnauthorizedAccessException | *destinationFileName* menentukan file yang hanya-baca dan akses tidak dapat dibaca.-or- jalur menentukan direktori.-or- Pemanggil tidak memiliki izin yang diperlukan. |
| NotSupportedException | *destinationFileName* berada dalam format yang tidak valid. |
| FileNotFoundException | Berkas tidak ditemukan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Catatan

Dimungkinkan untuk menyimpan arsip ke jalur yang sama dengan tempat ia dimuat. Namun, ini tidak disarankan karena pendekatan ini menggunakan penyalinan ke file sementara.

## Contoh

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("entry1", "data.bin");        
    archive.Save("myarchive.tar");
}       
```

### Lihat Juga

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


