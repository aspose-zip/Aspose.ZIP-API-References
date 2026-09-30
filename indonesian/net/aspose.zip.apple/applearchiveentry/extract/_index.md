---
title: "AppleArchiveEntry.Extract"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "AppleArchiveEntry metode. Mengekstrak entri ke sistem file menggunakan jalur yang diberikan"
type: docs
weight: 50
url: /id/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Mengekstrak entri ke sistem file menggunakan jalur yang disediakan.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| path | String | Jalur ke file tujuan. Jika file sudah ada, akan ditimpa. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| InvalidDataException | Checksum atau digest yang disimpan untuk entri tidak cocok dengan data yang diekstrak. |
| InvalidOperationException | Entri ini termasuk dalam arsip yang disiapkan untuk komposisi, atau data entri tidak dapat dibuka dari aliran arsip yang tidak dapat dipindai. |
| NotSupportedException | Entri ini termasuk dalam Apple Archive solid atau menggunakan metode kompresi yang tidak didukung. |
| ObjectDisposedException | Aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

### Lihat Juga

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Mengekstrak entri ke aliran yang disediakan.

```csharp
public void Extract(Stream destination)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tujuan | Stream | Stream tujuan. Harus dapat ditulis. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *destination* adalah `null`. |
| ArgumentException | *destination* tidak mendukung penulisan. |
| InvalidDataException | Checksum atau digest yang disimpan untuk entri tidak cocok dengan data yang diekstrak. |
| InvalidOperationException | Entri ini termasuk dalam arsip yang disiapkan untuk komposisi, atau data entri tidak dapat dibuka dari aliran arsip yang tidak dapat dipindai. |
| NotSupportedException | Entri ini termasuk dalam Apple Archive solid atau menggunakan metode kompresi yang tidak didukung. |
| ObjectDisposedException | Aliran sumber telah dibuang. |
| IOException | Terjadi kesalahan I/O. |

### Lihat Juga

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


