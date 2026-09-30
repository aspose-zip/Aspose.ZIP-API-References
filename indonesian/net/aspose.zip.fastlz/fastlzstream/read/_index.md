---
title: "FastLZStream.Read"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode FastLZStream. Membaca urutan byte dari aliran dan memajukan posisi dalam aliran sebesar jumlah byte yang dibaca. Tidak didukung"
type: docs
weight: 90
url: /id/net/aspose.zip.fastlz/fastlzstream/read/
---
## FastLZStream.Read method

Membaca urutan byte dari aliran dan memajukan posisi dalam aliran sebesar jumlah byte yang dibaca. Tidak didukung.

```csharp
public override int Read(byte[] buffer, int offset, int count)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| buffer | Byte[] | Array byte. Ketika metode ini mengembalikan, buffer berisi array byte yang ditentukan dengan nilai antara offset dan (offset + count - 1) diganti oleh byte yang dibaca dari sumber saat ini. |
| offset | Int32 | Offset byte berbasis nol dalam buffer di mana mulai menyimpan data yang dibaca dari aliran saat ini. |
| count | Int32 | Jumlah maksimum byte yang akan dibaca dari aliran saat ini. |

### Nilai Kembalian

Total jumlah byte yang dibaca ke dalam buffer. Ini dapat lebih sedikit daripada jumlah byte yang diminta jika byte tersebut tidak tersedia saat ini, atau nol (0) jika akhir aliran telah tercapai.

### Pengecualian

| exception | kondisi |
| --- | --- |
| NotSupportedException | Operasi tidak didukung. |

### Lihat Juga

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


