---
title: Class License
second_title: Aspose.ZIP untuk Referensi .NET API
description: Aspose.Zip.License kelas. Menyediakan metode untuk melisensikan komponen.
type: docs
weight: 260
url: /id/net/aspose.zip/license/
---
## License class

Menyediakan metode untuk melisensikan komponen.

```csharp
public class License
```

## Konstruktor

| Nama | Keterangan |
| --- | --- |
| [License](license/)() | Menginisialisasi instance baru dari`License` kelas. |

## Metode

| Nama | Keterangan |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Lisensi komponen. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Lisensi komponen. |

### Contoh

Dalam contoh ini, upaya akan dilakukan untuk menemukan file lisensi bernama MyLicense.lic di folder yang berisi  komponen, di folder yang berisi rakitan pemanggil, di folder rakitan entri, lalu di sumber daya tertanam rakitan pemanggil.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

file jar komponen:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Lihat juga

* ruang nama [Aspose.Zip](../../aspose.zip/)
* perakitan [Aspose.Zip](../../)


