---
title: CpioArchive.SaveGzipped
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: CpioArchive तरक. gzip कम्प्रेशन के सथ संग्रह क स्ट्रम में सहेजत है.
type: docs
weight: 90
url: /hi/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

gzip कम्प्रेशन के साथ संग्रह को स्ट्रीम में सहेजता है.

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| output | Stream | गंतव्य धारा। |
| cpioFormat | CpioFormat | cpio हैडर प्रारूप को परिभाषित करता है। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *output* शून्य है। |
| ArgumentException | *output* लिखने योग्य नहीं है। |

### टिप्पणियों

*output*लिखने योग्य होना चाहिए।

### उदाहरण

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### यह सभी देखें

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

आर्काइव को फ़ाइल में gzip कम्प्रेशन के साथ पथ द्वारा सहेजता है.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| cpioFormat | CpioFormat | cpio हैडर प्रारूप को परिभाषित करता है। |

### उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### यह सभी देखें

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)


