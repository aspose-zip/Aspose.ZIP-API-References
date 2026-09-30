---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode Lz4Archive. Mengekstrak arsip ke file berdasarkan jalur."
type: docs
weight: 30
url: /id/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Mengekstrak arsip ke file berdasarkan jalur.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

### Nilai Kembalian

Info tentang file yang diekstrak.

### Pengecualian

| exception | kondisi |
| --- | --- |
| EndOfStreamException | Aliran sumber terlalu pendek. |
| InvalidDataException | Byte yang salah ditemukan saat mendekode. |
| NotSupportedException | Versi LZ4 ini tidak didukung. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |
| InvalidOperationException | Arsip telah dipersiapkan untuk komposisi. |

### Lihat Juga

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Mengekstrak arsip ke aliran yang disediakan.

```csharp
public void Extract(Stream destination)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | Stream | Stream tujuan. Harus dapat ditulis. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentException | *destination* tidak mendukung penulisan. |
| EndOfStreamException | Aliran sumber terlalu pendek. |
| InvalidDataException | Byte yang salah ditemukan saat mendekode. |
| NotSupportedException | Versi LZ4 ini tidak didukung. |
| InvalidOperationException | Arsip telah dipersiapkan untuk komposisi. |
| OperationCanceledException | Di .NET Framework 4.0 ke atas: Dilempar ketika ekstraksi dibatalkan melalui token pembatalan yang disediakan. |
| ObjectDisposedException | Arsip telah dibuang dan tidak dapat digunakan. |

## Contoh

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Lihat Juga

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


