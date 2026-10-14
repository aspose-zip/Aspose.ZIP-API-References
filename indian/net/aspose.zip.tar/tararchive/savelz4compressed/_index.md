---
title: "TarArchive.SaveLZ4Compressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "TarArchive मेथड। LZ4 संपीड़न के साथ स्ट्रीम में संग्रह सहेजता है"
type: docs
weight: 170
url: /hi/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

LZ4 संपीड़न के साथ स्ट्रीम में संग्रह सहेजता है।

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| *output* null है। | स्ट्रीम | गंतव्य स्ट्रीम। |
| फ़ॉर्मेट | Nullable`1 | tar हेडर फ़ॉर्मेट को परिभाषित करता है। जब संभव हो तो Null मान को USTar माना जाएगा। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *output* लिखने योग्य नहीं है। |
| ArgumentException | आर्काइव निकासी के लिए तैयार है। - या - स्रोत प्रदान नहीं किया गया था। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता |
| IOException | एक I/O त्रुटि हुई। |

## टिप्पणियाँ

*output* must be writable.

## उदाहरण

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### संबंधित देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

LZ4 संपीड़न के साथ पथ द्वारा फ़ाइल में संग्रह सहेजता है।

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | बनाए जाने वाले अभिलेख का पथ। यदि निर्दिष्ट फ़ाइल नाम मौजूदा फ़ाइल की ओर संकेत करता है, तो उसे अधिलेखित कर दिया जाएगा। |
| फ़ॉर्मेट | Nullable`1 | tar हेडर फ़ॉर्मेट को परिभाषित करता है। जब संभव हो तो Null मान को USTar माना जाएगा। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| UnauthorizedAccessException | कॉलर के पास आवश्यक अनुमति नहीं है। -या- *path* ने केवल-पढ़ने योग्य फ़ाइल या निर्देशिका निर्दिष्ट की है। |
| ArgumentException | *path* शून्य-लंबाई की स्ट्रिंग है, केवल खाली स्थान रखती है, या InvalidPathChars द्वारा परिभाषित एक या अधिक अमान्य अक्षर रखती है। |
| ArgumentNullException | *path* शून्य है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| DirectoryNotFoundException | निर्दिष्ट *path* अमान्य है, (उदाहरण के लिए, यह एक अनमैप्ड ड्राइव पर है)। |
| NotSupportedException | *path* अमान्य प्रारूप में है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता |
| IOException | एक I/O त्रुटि हुई। |

## उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### संबंधित देखें

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


