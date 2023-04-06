---
title: Bzip2Archive.Save
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Bzip2Archive तरक. संग्रह क प्रदन क गई स्ट्रम में सहेजत है
type: docs
weight: 50
url: /hi/net/aspose.zip.bzip2/bzip2archive/save/
---
## Save(Stream, Bzip2SaveOptions) {#save}

संग्रह को प्रदान की गई स्ट्रीम में सहेजता है।

```csharp
public void Save(Stream outputStream, Bzip2SaveOptions saveOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| outputStream | Stream | गंतव्य धारा। |
| saveOptions | Bzip2SaveOptions | bzip2 संग्रह को सहेजने के विकल्प। यदि निर्दिष्ट नहीं है, तो 900 Kb ब्लॉक आकार का उपयोग किया जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| InvalidOperationException | संग्रहीत किए जाने वाले डेटा का स्रोत प्रदान नहीं किया गया है। |
| ArgumentException | *outputStream* लिखने योग्य नहीं है। |
| UnauthorizedAccessException | फ़ाइल स्रोत केवल पढ़ने के लिए है या एक निर्देशिका है। |
| DirectoryNotFoundException | निर्दिष्ट फ़ाइल स्रोत पथ अमान्य है, जैसे किसी अनमैप्ड ड्राइव पर होना। |
| IOException | फ़ाइल स्रोत पहले से ही खुला है। |

### टिप्पणियों

*outputStream*लिखने योग्य होना चाहिए।

### उदाहरण

एचटीटीपी रिस्पॉन्स स्ट्रीम में कंप्रेस्ड डेटा लिखता है।

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### यह सभी देखें

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)

---

## Save(string, Bzip2SaveOptions) {#save_1}

प्रदान की गई गंतव्य फ़ाइल में संग्रह सहेजता है.

```csharp
public void Save(string destinationFileName, Bzip2SaveOptions saveOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| destinationFileName | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| saveOptions | Bzip2SaveOptions | bzip2 संग्रह को सहेजने के विकल्प। यदि निर्दिष्ट नहीं है, तो 900 Kb ब्लॉक आकार का उपयोग किया जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *destinationFileName* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *destinationFileName* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*destinationFileName* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*destinationFileName*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*destinationFileName* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### उदाहरण

फ़ाइल करने के लिए संपीड़ित डेटा लिखता है।

```csharp
using (var archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.bz2");
}
```

### यह सभी देखें

* class [Bzip2SaveOptions](../../bzip2saveoptions/)
* class [Bzip2Archive](../)
* नाम स्थान [Aspose.Zip.Bzip2](../../bzip2archive/)
* सभा [Aspose.Zip](../../../)


