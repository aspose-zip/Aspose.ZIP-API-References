---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "CpioArchive मेथड। Z संपीड़न के साथ आर्काइव को स्ट्रीम में सहेजता है।"
type: docs
weight: 130
url: /hi/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

आर्काइव को Z संपीड़न के साथ स्ट्रीम में सहेजता है।

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| *output* null है। | स्ट्रीम | गंतव्य स्ट्रीम। |
| cpioFormat | CpioFormat | cpio हेडर फ़ॉर्मेट को परिभाषित करता है। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *output* लिखने योग्य नहीं है। |
| ArgumentException | आर्काइव निकासी के लिए तैयार है। - या - स्रोत प्रदान नहीं किया गया था। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

*output* must be writable.

## उदाहरण

```csharp
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

आर्काइव को Z संपीड़न के साथ पथ पर सहेजता है।

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, (उदाहरण के लिए, यह अनमैप्ड ड्राइव पर है)। |
| IOException | एक I/O त्रुटि हुई। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। |

## उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### संबंधित देखें

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


