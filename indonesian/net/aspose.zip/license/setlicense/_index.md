---
title: "License.SetLicense"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode License. Memberi lisensi pada komponen."
type: docs
weight: 20
url: /id/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

Melisensikan komponen.

```csharp
public void SetLicense(string licenseName)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| licenseName | String | Dapat berupa nama file lengkap atau singkat atau nama sumber daya tersemat. Gunakan string kosong untuk beralih ke mode evaluasi. |

## Catatan

Mencoba menemukan lisensi di lokasi berikut:

1. Jalur eksplisit.

2. Folder yang berisi assembly komponen Aspose.

3. Folder yang berisi assembly pemanggil klien.

4. Folder yang berisi assembly entri (startup).

5. Sumber daya tersemat dalam assembly pemanggil klien.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Jalur eksplisit.

2. Sumber daya tersemat dalam assembly pemanggil klien.

2. Folder yang berisi file JAR komponen Aspose.

3. Folder yang berisi file JAR pemanggil klien.

## Contoh

Dalam contoh ini, akan dicoba untuk menemukan berkas lisensi bernama MyLicense.lic di folder yang berisi komponen, di folder yang berisi assembly pemanggil, di folder assembly entri, dan kemudian di sumber daya tersemat dari assembly pemanggil.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

berkas jar komponen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Lihat Juga

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)

---

## SetLicense(Stream) {#setlicense}

Melisensikan komponen.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran yang berisi lisensi. |

## Catatan

Gunakan metode ini untuk memuat lisensi dari aliran.

## Contoh

```csharp
[C#]

License license = new License();
license.SetLicense(myStream);


[Visual Basic]

Dim license as License = new License
license.SetLicense(myStream)

License license = new License();
license.setLicense(myStream);
```

### Lihat Juga

* class [License](../)
* namespace [Aspose.Zip](../../license/)
* assembly [Aspose.Zip](../../../)


