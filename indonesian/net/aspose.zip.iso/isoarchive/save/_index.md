---
title: "IsoArchive.Save"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode IsoArchive. Menyimpan gambar ISO ke jalur yang ditentukan"
type: docs
weight: 70
url: /id/net/aspose.zip.iso/isoarchive/save/
---
## Save(string, IsoSaveOptions) {#save_1}

Menyimpan gambar ISO ke jalur yang ditentukan.

```csharp
public void Save(string path, IsoSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur tempat gambar ISO akan disimpan. |
| saveOptions | IsoSaveOptions | Opsi untuk menyimpan arsip ISO. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Dilempar ketika arsip tidak berada dalam mode penyuntingan. |
| ArgumentNullException | Dilempar ketika *path* bernilai null. |
| DirectoryNotFoundException | Dilempar ketika jalur yang ditentukan tidak valid, seperti berada pada drive yang tidak dipetakan. |
| IOException | Dilempar ketika file sudah terbuka. |
| UnauthorizedAccessException | Dilempar ketika akses ke *path* file ditolak. |
| PathTooLongException | Dilempar ketika *path* yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

Contoh berikut menunjukkan cara menyimpan arsip ISO ke sebuah file:

```csharp
// Buat arsip ISO kosong baru
using(IsoArchive isoArchive = new IsoArchive())
{
    // Tambahkan file ke arsip ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Simpan arsip ISO ke sebuah file
    isoArchive.Save("new_archive.iso");
}
```

### Lihat Juga

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, IsoSaveOptions) {#save}

Menyimpan gambar ISO ke aliran yang ditentukan.

```csharp
public void Save(Stream stream, IsoSaveOptions saveOptions = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Stream tempat gambar ISO akan disimpan. |
| saveOptions | IsoSaveOptions | Opsi untuk menyimpan arsip ISO. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Dilempar ketika arsip tidak berada dalam mode penyuntingan. |
| ArgumentNullException | Dilempar ketika *stream* bernilai null. |
| ArgumentException | Dilempar ketika *stream* tidak dapat ditulisi. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| IOException | Terjadi kesalahan I/O. |

## Contoh

Contoh berikut menunjukkan cara menyimpan arsip ISO ke stream memori:

```csharp

 // Buat arsip ISO kosong baru
 using(IsoArchive isoArchive = new IsoArchive())
 {
     // Tambahkan file ke arsip ISO
     isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

     // Simpan arsip ISO ke stream memori
     isoArchive.Save(memoryStream);
 }
```

### Lihat Juga

* class [IsoSaveOptions](../../isosaveoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


