---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode XarArchive. Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan"
type: docs
weight: 30
url: /id/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sourceDirectory | String | Direktori yang akan dikompresi. |
| compressionSettings | Boolean | Pengaturan kompresi yang digunakan untuk item [`XarEntry`](../../xarentry/) yang ditambahkan. |
| includeRootDirectory | XarCompressionSettings | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Instansi entri Xar.

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
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### Lihat Juga

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

Menambahkan ke arsip semua file dan direktori secara rekursif dalam direktori yang diberikan.

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| directory | DirectoryInfo | Direktori yang akan dikompresi. |
| compressionSettings | Boolean | Pengaturan kompresi yang digunakan untuk item [`XarEntry`](../../xarentry/) yang ditambahkan. |
| includeRootDirectory | XarCompressionSettings | Menunjukkan apakah menyertakan direktori akar itu sendiri atau tidak. |

### Nilai Kembalian

Instansi entri Xar.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *directory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *directory*. |
| IOException | *directory* berarti sebuah file, bukan sebuah direktori. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### Lihat Juga

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


