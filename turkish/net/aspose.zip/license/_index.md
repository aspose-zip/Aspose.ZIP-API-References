---
title: Class License
second_title: Aspose.ZIP for .NET API Referansı
description: Aspose.Zip.License sınıf. Bileşeni lisanslamak için yöntemler sağlar.
type: docs
weight: 260
url: /tr/net/aspose.zip/license/
---
## License class

Bileşeni lisanslamak için yöntemler sağlar.

```csharp
public class License
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [License](license/)() | Yeni bir örneğini başlatır.`License` sınıf. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Bileşeni lisanslar. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Bileşeni lisanslar. |

### Örnekler

Bu örnekte, içeren klasörde MyLicense.lic adlı bir lisans dosyası bulunmaya çalışılacaktır. bileşen, çağıran derlemeyi içeren klasörde, giriş derlemesinin klasöründe ve ardından çağıran derlemenin katıştırılmış kaynaklarında.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

bileşen jar dosyası:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Ayrıca bakınız

* ad alanı [Aspose.Zip](../../aspose.zip/)
* toplantı [Aspose.Zip](../../)


