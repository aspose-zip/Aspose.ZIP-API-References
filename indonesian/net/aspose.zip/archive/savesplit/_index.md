---
title: "Archive.SaveSplit"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Archive. Menyimpan arsip multivolume ke direktori tujuan yang diberikan"
type: docs
weight: 110
url: /id/net/aspose.zip/archive/savesplit/
---
## SaveSplit(string, SplitArchiveSaveOptions) {#savesplit_1}

Menyimpan arsip multi-volume ke direktori tujuan yang disediakan.

```csharp
public void SaveSplit(string destinationDirectory, SplitArchiveSaveOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| destinationDirectory | String | Jalur ke direktori tempat segmen arsip akan dibuat. |
| opsi | SplitArchiveSaveOptions | Opsi untuk menyimpan arsip, termasuk nama file. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidOperationException | Arsip ini dibuka dari sumber yang ada. |
| NotSupportedException | Arsip ini dikompresi dengan metode XZ dan juga dienkripsi. |
| ArgumentNullException | *destinationDirectory* bernilai null. |
| SecurityException | Pemanggil tidak memiliki izin yang diperlukan untuk mengakses direktori. |
| ArgumentException | *destinationDirectory* berisi karakter tidak valid seperti \", &gt;, &lt;, atau &#x7C;. |
| PathTooLongException | Jalur yang ditentukan melebihi panjang maksimum yang ditetapkan sistem. |
| ObjectDisposedException | Arsip telah dibuang. |
| DirectoryNotFoundException | Jalur yang ditentukan tidak valid, misalnya berada pada drive yang tidak dipetakan. |

## Catatan

Metode ini menyusun beberapa file (`n`) filename.z01, filename.z02, ..., filename.z(n-1), filename.zip.

Tidak dapat membuat arsip yang ada menjadi multi-volume.

## Contoh

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(@"C:\Folder",  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Lihat Juga

* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)

---

## SaveSplit(IVolumeStreamProvider, SplitArchiveSaveOptions) {#savesplit}

Menyimpan arsip multi-volume ke aliran yang disediakan oleh penyedia volume.

```csharp
public void SaveSplit(IVolumeStreamProvider volumeStreamProvider, SplitArchiveSaveOptions options)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| volumeStreamProvider | IVolumeStreamProvider | Penyedia aliran tujuan untuk volume arsip. |
| options | SplitArchiveSaveOptions | Opsi untuk menyimpan arsip. [`FileName`](../../../aspose.zip.saving/splitarchivesaveoptions/filename/) diabaikan. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *volumeStreamProvider* atau *options* bernilai null. |
| InvalidOperationException | Arsip ini dibuka dari sumber yang ada, atau penyedia mengembalikan aliran yang null atau tidak dapat ditulisi. |
| NotSupportedException | Arsip ini menggunakan kompresi XZ. |
| ObjectDisposedException | Arsip telah dibuang. |

## Catatan

Aliran yang disediakan tidak perlu mendukung pencarian.

Setiap volume yang selesai dibersihkan, diteruskan ke [`VolumeCompleted`](../../../aspose.zip.saving/ivolumestreamprovider/volumecompleted/), dan kemudian dibuang.

Tidak dapat membuat arsip yang ada menjadi multi-volume. Kompresi XZ tidak didukung oleh overload ini karena memerlukan pencarian.

## Contoh

```csharp
using (Archive archive = new Archive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.SaveSplit(provider,  new SplitArchiveSaveOptions("volume", 65536));
}
```

### Lihat Juga

* interface [IVolumeStreamProvider](../../../aspose.zip.saving/ivolumestreamprovider/)
* class [SplitArchiveSaveOptions](../../../aspose.zip.saving/splitarchivesaveoptions/)
* class [Archive](../)
* namespace [Aspose.Zip](../../archive/)
* assembly [Aspose.Zip](../../../)


