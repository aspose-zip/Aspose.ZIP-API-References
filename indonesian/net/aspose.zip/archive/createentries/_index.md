---
title: "Archive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode arsip. Tambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan."
type: docs
weight: 50
url: /id/net/aspose.zip/archive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

Tambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public Archive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
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
| DirectoryNotFoundException | Jalur ke *directory* tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *directory*. |
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| ArgumentNullException | *directory* bernilai `null`. |

## Contoh

```csharp
using (Archive archive = new Archive())
{
    DirectoryInfo folder = new DirectoryInfo("C:\folder");
    archive.CreateEntries(folder);
    archive.Save("folder.zip");
}
```

### Lihat Juga

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

Tambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public Archive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
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
| ObjectDisposedException | Dilempar jika arsip telah dibuang. |
| ArgumentException | *sourceDirectory* berisi karakter tidak valid seperti ", &lt;, &gt;, atau &#x7C;. |
| ArgumentNullException | *sourceDirectory* adalah `null`. |
| PathTooLongException | Jalur, nama file, atau keduanya yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |

## Contoh

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntries("C:\folder");
    archive.Save("folder.zip");
}
```

### Lihat Juga

* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


