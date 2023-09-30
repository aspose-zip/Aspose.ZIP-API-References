---
title: TarArchive.FromLZip
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. दए गए अर्क lzip आर्कइव और कंपज़ करते हैंTarArchive नकले गए डेट से.
type: docs
weight: 30
url: /hi/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

दिए गए अर्क lzip आर्काइव और कंपोज़ करते हैं[`TarArchive`](../) निकाले गए डेटा से.

महत्वपूर्ण: lzip संग्रह इस पद्धति के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री को आंतरिक रूप से रखा जाता है। स्मृति खपत से सावधान रहें।

```csharp
public static TarArchive FromLZip(Stream source)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| source | Stream | संग्रह का स्रोत। |

### प्रतिलाभ की मात्रा

का एक उदाहरण[`TarArchive`](../)

### टिप्पणियों

कम्प्रेशन एल्गोरिथम की प्रकृति से Lzip एक्सट्रैक्शन स्ट्रीम खोजने योग्य नहीं है। टार आर्काइव मनमाना रिकॉर्ड निकालने की सुविधा प्रदान करता है, इसलिए इसे हुड के तहत सीकेबल स्ट्रीम को संचालित करना पड़ता है।

### यह सभी देखें

* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

दिए गए अर्क lzip आर्काइव और कंपोज़ करते हैं[`TarArchive`](../) निकाले गए डेटा से.

महत्वपूर्ण: lzip संग्रह इस पद्धति के भीतर पूरी तरह से निकाला जाता है, इसकी सामग्री को आंतरिक रूप से रखा जाता है। स्मृति खपत से सावधान रहें।

```csharp
public static TarArchive FromLZip(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | संग्रह फ़ाइल का पथ। |

### प्रतिलाभ की मात्रा

का एक उदाहरण[`TarArchive`](../)

### टिप्पणियों

कम्प्रेशन एल्गोरिथम की प्रकृति से Lzip एक्सट्रैक्शन स्ट्रीम खोजने योग्य नहीं है। टार आर्काइव मनमाना रिकॉर्ड निकालने की सुविधा प्रदान करता है, इसलिए इसे हुड के तहत सीकेबल स्ट्रीम को संचालित करना पड़ता है।

### यह सभी देखें

* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

