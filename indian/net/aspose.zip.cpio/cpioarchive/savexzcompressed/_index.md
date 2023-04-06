---
title: CpioArchive.SaveXzCompressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: CpioArchive तरक. संग्रह क xz संपड़न के सथ स्ट्रम में सहेजत है.
type: docs
weight: 100
url: /hi/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

संग्रह को xz संपीड़न के साथ स्ट्रीम में सहेजता है.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| output | Stream | गंतव्य धारा। |
| cpioFormat | CpioFormat | cpio हैडर प्रारूप को परिभाषित करता है। |
| settings | XzArchiveSettings | विशेष xz संग्रह सेटिंग का सेट: शब्दकोश आकार, ब्लॉक आकार, चेक प्रकार। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *output* शून्य है। |
| ArgumentException | *output* लिखने योग्य नहीं है। |

### टिप्पणियों

*output*धारा लिखने योग्य होनी चाहिए।

### उदाहरण

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### यह सभी देखें

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

संग्रह को xz संपीड़न के साथ पथ द्वारा पथ में सहेजता है.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| cpioFormat | CpioFormat | cpio हैडर प्रारूप को परिभाषित करता है। |
| settings | XzArchiveSettings | विशेष xz संग्रह सेटिंग का सेट: शब्दकोश आकार, ब्लॉक आकार, चेक प्रकार। |

### उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### यह सभी देखें

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)


