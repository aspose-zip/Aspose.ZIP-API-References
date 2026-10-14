---
title: "Bzip2SaveOptions.Bzip2SaveOptions"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Konstruktor Bzip2SaveOptions. Menginisialisasi instance baru dari kelas Bzip2SaveOptions"
type: docs
weight: 10
url: /id/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Menginisialisasi instance baru dari kelas [`Bzip2SaveOptions`](../).

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| blockSize | Int32 | Ukuran blok dalam ratusan kilobyte. |

### Pengecualian

| exception | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran blok tidak berada dalam rentang yang valid. |

## Contoh

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### Lihat Juga

* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Menginisialisasi instance baru dari kelas [`Bzip2SaveOptions`](../) dengan ukuran blok default, yaitu 9 ratus kilobyte.

```csharp
public Bzip2SaveOptions()
```

## Contoh

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### Lihat Juga

* class [Bzip2SaveOptions](../)
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


