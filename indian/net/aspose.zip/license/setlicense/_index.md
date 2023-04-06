---
title: License.SetLicense
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: License तरक. घटक क लइसेंस देत है
type: docs
weight: 20
url: /hi/net/aspose.zip/license/setlicense/
---
## SetLicense(string) {#setlicense_1}

घटक को लाइसेंस देता है।

```csharp
public void SetLicense(string licenseName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| licenseName | String | एक पूर्ण या छोटा फ़ाइल नाम या एम्बेडेड संसाधन का नाम हो सकता है। मूल्यांकन मोड पर स्विच करने के लिए एक खाली स्ट्रिंग का उपयोग करें। |

### टिप्पणियों

निम्न स्थानों में लाइसेंस ढूँढने का प्रयास करता है:

1. स्पष्ट पथ।

2. वह फ़ोल्डर जिसमें Aspose घटक असेंबली है।

3. क्लाइंट की कॉलिंग असेंबली वाला फ़ोल्डर।

4. फ़ोल्डर जिसमें प्रविष्टि (स्टार्टअप) असेंबली है।

5. ग्राहक की कॉलिंग असेंबली में एक एम्बेडेड संसाधन।

**टिप्पणी:**.NET कॉम्पैक्ट फ्रेमवर्क पर, केवल इन स्थानों में लाइसेंस खोजने की कोशिश करता है:

1. स्पष्ट पथ।

2. क्लाइंट की कॉलिंग असेंबली में एक एम्बेडेड संसाधन।

2. वह फ़ोल्डर जिसमें Aspose घटक JAR फ़ाइल है।

3. वह फ़ोल्डर जिसमें क्लाइंट की कॉलिंग JAR फ़ाइल होती है।

### उदाहरण

इस उदाहरण में, MyLicense.lic नामक लाइसेंस फ़ाइल को फ़ोल्डर में खोजने का प्रयास किया जाएगा जिसमें है घटक, कॉलिंग असेंबली वाले फ़ोल्डर में, एंट्री असेंबली के फ़ोल्डर में और फिर कॉलिंग असेंबली के एम्बेडेड संसाधनों में।

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");
```

घटक जार फ़ाइल:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### यह सभी देखें

* class [License](../)
* नाम स्थान [Aspose.Zip](../../license/)
* सभा [Aspose.Zip](../../../)

---

## SetLicense(Stream) {#setlicense}

घटक को लाइसेंस देता है।

```csharp
public void SetLicense(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| stream | Stream | एक धारा जिसमें लाइसेंस शामिल है। |

### टिप्पणियों

स्ट्रीम से लाइसेंस लोड करने के लिए इस विधि का उपयोग करें।

### उदाहरण

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

### यह सभी देखें

* class [License](../)
* नाम स्थान [Aspose.Zip](../../license/)
* सभा [Aspose.Zip](../../../)


