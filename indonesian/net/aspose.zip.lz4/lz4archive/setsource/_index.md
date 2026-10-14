---
title: "Lz4Archive.SetSource"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Lz4Archive. Menetapkan konten yang akan dikompresi dalam arsip."
type: docs
weight: 70
url: /id/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(Stream source)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| source | Stream | Stream input untuk arsip. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Lihat Juga

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fileInfo | FileInfo | Referensi ke file yang akan dikompresi. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

Buka arsip dari stream dan ekstrak ke `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Lihat Juga

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tarArchive | TarArchive | Arsip Tar yang akan dikompres. |
| format | TarFormat | Mendefinisikan format header tar. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip ini telah dipersiapkan untuk ekstraksi. |

## Catatan

Gunakan metode ini untuk menyusun arsip tar.lz4 gabungan.

## Contoh

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Lihat Juga

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Menetapkan konten yang akan dikompresi dalam arsip.

```csharp
public void SetSource(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file yang akan dikompres. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| InvalidOperationException | Arsip ini telah dipersiapkan untuk ekstraksi. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

Buka arsip dari file dengan jalur dan ekstrak ke `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Lihat Juga

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


