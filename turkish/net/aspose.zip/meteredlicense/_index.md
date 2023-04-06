---
title: Class MeteredLicense
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.MeteredLicense sınıf. Ölçülen anahtarı ayarlamak için yöntemler sağlar.
type: docs
weight: 290
url: /tr/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Ölçülen anahtarı ayarlamak için yöntemler sağlar.

```csharp
public class MeteredLicense
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | Bu sınıfın yeni bir örneğini başlatır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Tarifeli genel ve özel anahtarı ayarlar. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Tüketim kredisi alır. |

### Notlar

Önemli: ölçülü lisans ile kendi kendine açılan zip arşivleri oluşturamazsınız.

### Örnekler

Bu örnekte, ölçülü genel ve özel anahtar ayarlanmaya çalışılacaktır.

```csharp
MeteredLicense matered = new MeteredLicense();
matered.SetMeteredKey("PublicKey", "PrivateKey");
```

### Ayrıca bakınız

* ad alanı [Aspose.Zip](../../aspose.zip/)
* toplantı [Aspose.Zip](../../)


