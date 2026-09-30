---
title: "CpioArchive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CpioArchive. Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan"
type: docs
weight: 30
url: /id/net/aspose.zip.cpio/cpioarchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public CpioArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | String | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Instansi entri Cpio.

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
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(cpioFile);
    }
}
```

### Lihat Juga

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public CpioArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori yang akan dikompresi. |
| includeRootDirectory | Boolean | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Instansi entri Cpio.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *directory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *directory*. |
| IOException | *directory* berarti sebuah file, bukan sebuah direktori. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (FileStream cpioFile = File.Open("archive.cpio", FileMode.Create))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(cpioFile);
    }
}
```

### Lihat Juga

* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


