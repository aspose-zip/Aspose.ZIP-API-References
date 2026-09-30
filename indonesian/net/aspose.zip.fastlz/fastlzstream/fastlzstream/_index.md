---
title: "FastLZStream.FastLZStream"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor FastLZStream. Menginisialisasi instance baru dari kelas FastLZStream yang dipersiapkan untuk kompresi"
type: docs
weight: 10
url: /id/net/aspose.zip.fastlz/fastlzstream/fastlzstream/
---
## FastLZStream constructor

Menginisialisasi instance baru dari kelas [`FastLZStream`](../) yang disiapkan untuk kompresi.

```csharp
public FastLZStream(Stream stream, int compressionLevel)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Stream untuk menyimpan data terkompresi. |
| compressionLevel | Int32 | Gunakan 1 untuk kompresi lebih cepat, gunakan 2 untuk rasio kompresi yang lebih baik. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentNullException | *stream* bernilai null. |
| ArgumentException | *stream* tidak mendukung penulisan. |
| ArgumentOutOfRangeException | *compressionLevel* lebih dari 2 atau kurang dari 1. |

### Lihat Juga

* class [FastLZStream](../)
* namespace [Aspose.Zip.FastLZ](../../fastlzstream/)
* assembly [Aspose.Zip](../../../)


