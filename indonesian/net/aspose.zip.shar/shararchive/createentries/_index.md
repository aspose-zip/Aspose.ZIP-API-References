---
title: "SharArchive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode SharArchive. Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan"
type: docs
weight: 30
url: /id/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | String | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Instance entri Shar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceDirectory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *sourceDirectory*. |
| ArgumentException | *sourceDirectory* berisi karakter tidak valid seperti ", &lt;, &gt;, atau &#x7C;. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. Jalur, nama file, atau keduanya yang ditentukan terlalu panjang. |
| IOException | *sourceDirectory* berarti sebuah file, bukan sebuah direktori. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Instance entri Shar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *directory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *directory*. |
| IOException | *directory* berarti sebuah file, bukan sebuah direktori. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### Lihat Juga

* class [SharArchive](../)
* namespace [Aspose.Zip.Shar](../../shararchive/)
* assembly [Aspose.Zip](../../../)


