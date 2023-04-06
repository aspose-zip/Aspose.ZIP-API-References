---
title: Class License
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Aspose.Zip.License कक्ष. घटक क लइसेंस देने के तरके प्रदन करत है
type: docs
weight: 260
url: /hi/net/aspose.zip/license/
---
## License class

घटक को लाइसेंस देने के तरीके प्रदान करता है।

```csharp
public class License
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [License](license/)() | का एक नया उदाहरण प्रारंभ करता है`License` कक्षा। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | घटक को लाइसेंस देता है। |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | घटक को लाइसेंस देता है। |

### उदाहरण

इस उदाहरण में, MyLicense.lic नामक लाइसेंस फ़ाइल को फ़ोल्डर में खोजने का प्रयास किया जाएगा जिसमें है घटक, कॉलिंग असेंबली वाले फ़ोल्डर में, एंट्री असेंबली के फ़ोल्डर में और फिर कॉलिंग असेंबली के एम्बेडेड संसाधनों में।

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

घटक जार फ़ाइल:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### यह सभी देखें

* नाम स्थान [Aspose.Zip](../../aspose.zip/)
* सभा [Aspose.Zip](../../)


