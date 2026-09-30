---
title: "TarArchive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode TarArchive. Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan"
type: docs
weight: 100
url: /id/net/aspose.zip.tar/tararchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public TarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Arsip dengan entri yang telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Contoh

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(tarFile);
    }
}
```

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public TarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | String | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Arsip dengan entri yang telah disusun.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *sourceDirectory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *sourceDirectory*. |
| ArgumentException | *sourceDirectory* berisi karakter tidak valid seperti ", &lt;, &gt;, atau &#x7C;. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama file harus kurang dari 260 karakter. Jalur, nama file, atau keduanya yang ditentukan terlalu panjang. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan |

## Contoh

```csharp
using (FileStream tarFile = File.Open("archive.tar", FileMode.Create))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(tarFile);
    }
}
```

### Lihat Juga

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


