---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP untuk Referensi .NET API
description: Bzip2SaveOptions konstruktor. Menginisialisasi instance baru dariBzip2SaveOptions kelas.
type: docs
weight: 10
url: /id/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Menginisialisasi instance baru dari[`Bzip2SaveOptions`](../) kelas.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Parameter | Jenis | Keterangan |
| --- | --- | --- |
| blockSize | Int32 | Ukuran blok dalam ratusan kilobyte. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentOutOfRangeException | Ukuran blok tidak dalam rentang yang valid. |

### Contoh

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

### Lihat juga

* class [Bzip2SaveOptions](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* perakitan [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Menginisialisasi instance baru dari[`Bzip2SaveOptions`](../) kelas dengan ukuran blok default, sama dengan 9 ratus kilobyte.

```csharp
public Bzip2SaveOptions()
```

### Contoh

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

### Lihat juga

* class [Bzip2SaveOptions](../)
* ruang nama [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* perakitan [Aspose.Zip](../../../)


