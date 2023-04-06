---
title: TarArchive.SaveXzCompressed
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. संग्रह क xz संपड़न के सथ स्ट्रम में सहेजत है.
type: docs
weight: 150
url: /hi/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

संग्रह को xz संपीड़न के साथ स्ट्रीम में सहेजता है.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| output | Stream | गंतव्य धारा। |
| format | Nullable`1 | टार हेडर प्रारूप को परिभाषित करता है। संभव होने पर शून्य मान को यूएसटार के रूप में माना जाएगा। |
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
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

संग्रह को xz संपीड़न के साथ पथ द्वारा पथ में सहेजता है.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | बनाए जाने वाले संग्रह का पथ. यदि निर्दिष्ट फ़ाइल नाम किसी मौजूदा फ़ाइल की ओर इशारा करता है, तो इसे अधिलेखित कर दिया जाएगा। |
| format | Nullable`1 | टार हेडर प्रारूप को परिभाषित करता है। संभव होने पर शून्य मान को यूएसटार के रूप में माना जाएगा। |
| settings | XzArchiveSettings | विशेष xz संग्रह सेटिंग का सेट: शब्दकोश आकार, ब्लॉक आकार, चेक प्रकार। |

### उदाहरण

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### यह सभी देखें

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


