---
title: "MeteredLicense.SetMeteredKey"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Metode MeteredLicense. Mengatur kunci publik dan privat bermeter"
type: docs
weight: 30
url: /id/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Mengatur kunci publik dan privat bermeter.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| publicKey | String | Kunci publik. |
| privateKey | String | Kunci privat. |

## Catatan

Jika Anda membeli lisensi bermeter, API ini harus dipanggil saat aplikasi dimulai, biasanya ini sudah cukup. Namun, jika metered gagal mengunggah data konsumsi selama periode 24 jam, lisensi akan diatur ke status evaluasi. Untuk menghindari hal tersebut, Anda harus secara teratur memeriksa status lisensi. Jika statusnya masih evaluasi, panggil kembali API ini.

### Lihat Juga

* class [MeteredLicense](../)
* namespace [Aspose.Zip](../../meteredlicense/)
* assembly [Aspose.Zip](../../../)


