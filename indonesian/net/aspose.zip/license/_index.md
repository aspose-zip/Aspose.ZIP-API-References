---
title: "Kelas License"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.License. Menyediakan metode untuk melisensikan komponen"
type: docs
weight: 660
url: /id/net/aspose.zip/license/
---
## License class

Menyediakan metode untuk melisensikan komponen.

```csharp
public sealed class License
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [License](license/)() | Menginisialisasi instance baru dari kelas `License`. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Melisensikan komponen. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Melisensikan komponen. |

## Contoh

Dalam contoh ini, akan dicoba untuk menemukan berkas lisensi bernama MyLicense.lic di folder yang berisi komponen, di folder yang berisi assembly pemanggil, di folder assembly entri, dan kemudian di sumber daya tersemat dari assembly pemanggil.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

berkas jar komponen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Lihat Juga

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


