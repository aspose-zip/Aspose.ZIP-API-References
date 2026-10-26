---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "CpioArchive मेथड। LZMA संपीड़न के साथ आर्काइव को स्ट्रीम में सहेजता है।"
type: docs
weight: 110
url: /hi/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

आर्काइव को LZMA संपीड़न के साथ स्ट्रीम में सहेजता है।

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| *output* null है। | स्ट्रीम | गंतव्य स्ट्रीम। |
| cpioFormat | CpioFormat | cpio हेडर फ़ॉर्मेट को परिभाषित करता है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| NotSupportedException | स्ट्रीम लिखने का समर्थन नहीं करता, या स्ट्रीम पहले ही बंद हो चुका है। |

## टिप्पणियाँ

*output* must be writable.

महत्वपूर्ण: cpio आर्काइव इस विधि में निर्मित और फिर संपीड़ित किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

## उदाहरण

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### संबंधित देखें

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

आर्काइव को पथ द्वारा फ़ाइल में lzma संपीड़न के साथ सहेजता है।

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |
| cpioFormat | CpioFormat | cpio हेडर फ़ॉर्मेट को परिभाषित करता है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentNullException | *path* `null` है। |
| Exception | रनटाइम त्रुटि होने पर फेंका जाता है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, (उदाहरण के लिए, यह अनमैप्ड ड्राइव पर है)। |
| IOException | एक I/O त्रुटि हुई। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। |
| UnauthorizedAccessException | कॉलर के पास आवश्यक अनुमति नहीं है। -या- *path* ने केवल-पढ़ने योग्य फ़ाइल या निर्देशिका निर्दिष्ट की है। |

## टिप्पणियाँ

महत्वपूर्ण: cpio आर्काइव इस विधि में निर्मित और फिर संपीड़ित किया जाता है, इसकी सामग्री आंतरिक रूप से रखी जाती है। मेमोरी उपयोग का ध्यान रखें।

## उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### संबंधित देखें

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


