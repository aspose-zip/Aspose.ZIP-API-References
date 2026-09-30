---
title: "LzmaCompressionSettings.LzmaCompressionSettings"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor LzmaCompressionSettings. Menginisialisasi instance baru dari kelas LzmaCompressionSettings dengan parameter default"
type: docs
weight: 10
url: /id/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings() {#constructor}

Menginisialisasi instance baru dari kelas [`LzmaCompressionSettings`](../) dengan parameter default.

```csharp
public LzmaCompressionSettings()
```

## Contoh

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Lihat Juga

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int, int, int) {#constructor_2}

Menginisialisasi instance baru dari kelas [`LzmaCompressionSettings`](../) dengan ukuran kamus yang ditentukan, jumlah byte cepat, dan jumlah bit konteks literal.

```csharp
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran kamus (buffer riwayat) dalam byte. Harus antara 4096 dan 1073741824. |
| numberOfFastBytes | Int32 | Jumlah byte yang digunakan untuk pencarian kecocokan cepat dalam algoritma LZMA. Dapat berada dalam rentang 5 hingga 273. |
| literalContextBits | Int32 | Mengatur jumlah bit konteks literal (bit tinggi dari literal sebelumnya). Nilainya dapat berada dalam rentang 0 hingga 8. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Dilempar ketika salah satu argumen berada di luar rentang nilai yang diizinkan. |

### Lihat Juga

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int) {#constructor_1}

Menginisialisasi instance baru dari kelas [`LzmaCompressionSettings`](../) dengan ukuran kamus yang ditentukan, jumlah fast byte default sebesar 32, dan jumlah bit konteks literal sebesar 3.

```csharp
public LzmaCompressionSettings(int dictionarySize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dictionarySize | Int32 | Ukuran kamus (buffer riwayat) dalam byte. Harus antara 4096 dan 1073741824. |

### Lihat Juga

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


