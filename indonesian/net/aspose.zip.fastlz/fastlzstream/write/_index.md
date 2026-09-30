---
title: "FastLZStream.Write"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode FastLZStream. Menulis urutan byte ke aliran kompresi dan memajukan posisi saat ini dalam aliran ini sebesar jumlah byte yang ditulis."
type: docs
weight: 120
url: /id/net/aspose.zip.fastlz/fastlzstream/write/
---
## FastLZStream.Write method

Menulis urutan byte ke aliran kompresi dan memajukan posisi saat ini dalam aliran ini sebanyak jumlah byte yang ditulis.

```csharp
public override void Write(byte[] buffer, int offset, int count)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| buffer | Byte[] | Array byte. Metode ini menyalin count byte dari buffer ke aliran saat ini. |
| offset | Int32 | Offset byte berbasis nol dalam buffer di mana penyalinan byte ke aliran saat ini dimulai. |
| count | Int32 | Jumlah byte yang akan ditulis ke aliran saat ini. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ObjectDisposedException | Dilemparkan jika aliran telah dibuang. |
| ArgumentNullException | *buffer* adalah `null`. |

### Lihat Juga

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


