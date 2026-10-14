---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode ArjEntryPlain. Mengekstrak entri ke sistem file menggunakan path yang diberikan"
type: docs
weight: 40
url: /id/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

### Nilai Kembalian

Info file dari file yang disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null atau kosong. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| FileNotFoundException | Berkas tidak ditemukan. |
| InvalidDataException | Checksum tidak cocok untuk header atau data. - atau - Arsip rusak. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| NotImplementedException | Entri dikompresi dengan metode 4. |

## Contoh

Ekstrak dua entri dari arsip rar.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Lihat Juga

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Mengekstrak entri arsip ARJ ke sebuah file.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo untuk menyimpan data yang telah didekompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Header arsip dan informasi layanan tidak dibaca. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk membuka *fileInfo*. |
| ArgumentException | Path file kosong atau hanya berisi spasi. |
| FileNotFoundException | Berkas tidak ditemukan. |
| UnauthorizedAccessException | Path ke file bersifat read-only atau merupakan direktori. |
| ArgumentNullException | *fileInfo* bernilai null. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| InvalidDataException | Checksum tidak cocok untuk header atau data. - atau - Arsip rusak. |
| NotImplementedException | Entri dikompresi dengan metode 4. |

## Contoh

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Lihat Juga

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public void Extract(Stream destination)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | Stream | Stream tujuan. Harus dapat ditulis. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |
| InvalidDataException | Checksum tidak cocok untuk header atau data. - atau - Arsip rusak. |
| NotImplementedException | Entri dikompresi dengan metode 4. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |

### Lihat Juga

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


