---
title: "SevenZipLZMACompressionSettings.SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor SevenZipLZMACompressionSettings. Menginisialisasi instance baru dari kelas SevenZipLZMACompressionSettings dengan parameter default"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/sevenziplzmacompressionsettings/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings() {#constructor}

Menginisialisasi instance baru dari kelas [`SevenZipLZMACompressionSettings`](../) dengan parameter default.

```csharp
public SevenZipLZMACompressionSettings()
```

## Contoh

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save("result.7z");
}
```

### Lihat Juga

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int, int, int) {#constructor_2}

Menginisialisasi sebuah instance baru dari kelas [`SevenZipLZMACompressionSettings`](../) dengan ukuran kamus yang ditentukan, jumlah fast bytes, dan jumlah literal context bits.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, 
    int literalContextBits)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran kamus (buffer riwayat) dalam byte. Harus antara 4096 dan 1073741824, atau sama dengan nol untuk deteksi otomatis berdasarkan ukuran entri. |
| numberOfFastBytes | Int32 | Jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. Dapat berada dalam rentang 5 hingga 273. |
| literalContextBits | Int32 | Mengatur jumlah bit konteks literal (bit tinggi dari literal sebelumnya). Nilainya dapat berada dalam rentang 0 hingga 8. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Dilempar ketika salah satu argumen berada di luar rentang nilai yang diizinkan. |

### Lihat Juga

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int) {#constructor_1}

Menginisialisasi sebuah instance baru dari kelas [`SevenZipLZMACompressionSettings`](../) dengan ukuran kamus yang ditentukan, jumlah fast bytes sebesar 32, dan jumlah literal context bits sebesar 3.

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran kamus (buffer riwayat) dalam byte. Harus antara 4096 dan 1073741824, atau sama dengan nol untuk deteksi otomatis berdasarkan ukuran entri. |

### Lihat Juga

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


