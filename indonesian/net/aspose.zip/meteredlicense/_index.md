---
title: "Kelas MeteredLicense"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Kelas Aspose.Zip.MeteredLicense. Menyediakan metode untuk mengatur kunci bermeter."
type: docs
weight: 760
url: /id/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Menyediakan metode untuk mengatur kunci bermeter.

```csharp
public class MeteredLicense
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | Konstruktor default. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [ResetMeteredKey](../../aspose.zip/meteredlicense/resetmeteredkey/)() | Menghapus lisensi yang sebelumnya disiapkan. |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Mengatur kunci publik dan privat bermeter. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Mendapatkan kredit konsumsi. |
| static [GetConsumptionQuantity](../../aspose.zip/meteredlicense/getconsumptionquantity/)() | Mendapatkan ukuran file konsumsi. |

## Contoh

Dalam contoh ini, akan dicoba untuk mengatur kunci publik dan privat bermeter

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

berkas jar komponen:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### Lihat Juga

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


