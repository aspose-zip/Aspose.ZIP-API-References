---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode CabArchive. Membuat satu entri dalam arsip"
type: docs
weight: 40
url: /id/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Buat satu entri dalam arsip.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| path | String | Nama lengkap dari file baru, atau nama file relatif yang akan dikompres. |
| newEntrySettings | CabEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`CabEntry`](../../cabentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Cab.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *path* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses. |
| ArgumentException | *path* kosong, hanya berisi spasi, atau berisi karakter tidak valid. |
| UnauthorizedAccessException | Akses ke berkas *path* ditolak. |
| PathTooLongException | *path* yang ditentukan, nama berkas, atau keduanya melebihi panjang maksimum yang ditetapkan sistem. Misalnya, pada platform berbasis Windows, jalur harus kurang dari 248 karakter, dan nama berkas harus kurang dari 260 karakter. |
| NotSupportedException | Berkas di *path* mengandung titik dua (:) di tengah string. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi dan tidak dapat menambahkan entri. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan dalam parameter *path* tidak memengaruhi nama entri.

## Contoh

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Lihat Juga

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Buat satu entri dalam arsip.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| source | Stream | Aliran masukan untuk entri. |
| newEntrySettings | CabEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`CabEntry`](../../cabentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri Cab.

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi dan tidak dapat menambahkan entri. |
| ArgumentNullException | *name* bernilai null. |

## Contoh

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Lihat Juga

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Buat satu entri dalam arsip.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| fileInfo | FileInfo | Metadata file yang akan dikompresi. |
| newEntrySettings | CabEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`CabEntry`](../../cabentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri CAB.

### Pengecualian

| exception | kondisi |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* bersifat read-only atau merupakan direktori. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |
| IOException | Berkas sudah terbuka. |
| FileNotFoundException | *fileInfo* mewakili file yang tidak dapat ditemukan. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses *fileInfo*. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip telah dipersiapkan untuk ekstraksi dan tidak dapat menambahkan entri. |
| ArgumentNullException | *name* bernilai null. |

## Catatan

Nama entri hanya diatur melalui parameter *name*. Nama file yang diberikan pada parameter *fileInfo* tidak memengaruhi nama entri.

## Contoh

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Lihat Juga

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Buat satu entri dalam arsip.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | String | Nama entri. |
| streamProvider | Func`1 | Metode yang menyediakan aliran masukan untuk entri. |
| newEntrySettings | CabEntrySettings | Pengaturan kompresi dan enkripsi yang digunakan untuk item [`CabEntry`](../../cabentry/) yang ditambahkan. |

### Nilai Kembalian

Instansi entri CAB.

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Arsip diinstansiasi untuk dekompresi. - atau - Jumlah file telah mencapai batas. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| ArgumentException | *name* adalah null atau kosong. |

## Contoh

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Lihat Juga

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


