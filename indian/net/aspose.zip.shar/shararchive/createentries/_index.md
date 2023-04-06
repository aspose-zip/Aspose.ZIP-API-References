---
title: SharArchive.CreateEntries
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SharArchive तरक. द गई नर्देशक में सभ फइलं और नर्देशकओं क पुनरवर्त रूप से संग्रह में जड़त है
type: docs
weight: 30
url: /hi/net/aspose.zip.shar/shararchive/createentries/
---
## CreateEntries(string, bool) {#createentries_1}

दी गई निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

```csharp
public SharArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceDirectory | String | संपीड़ित करने के लिए निर्देशिका। |
| includeRootDirectory | Boolean | इंगित करता है कि रूट निर्देशिका को स्वयं शामिल करना है या नहीं। |

### प्रतिलाभ की मात्रा

Shar प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *sourceDirectory* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है*sourceDirectory*. |
| ArgumentException | *sourceDirectory* में अमान्य वर्ण हैं जैसे ", &lt;,&gt;, या &#x7C;। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। निर्दिष्ट पथ, फ़ाइल नाम, या दोनों बहुत लंबे हैं। |
| IOException | *sourceDirectory* फ़ाइल के लिए खड़ा है, निर्देशिका के लिए नहीं। |

### उदाहरण

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries("C:\folder", false);
        archive.Save(sharFile);
    }
}
```

### यह सभी देखें

* class [SharArchive](../)
* नाम स्थान [Aspose.Zip.Shar](../../shararchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool) {#createentries}

दी गई निर्देशिका में सभी फाइलों और निर्देशिकाओं को पुनरावर्ती रूप से संग्रह में जोड़ता है।

```csharp
public SharArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| directory | DirectoryInfo | संपीड़ित करने के लिए निर्देशिका। |
| includeRootDirectory | Boolean | इंगित करता है कि रूट निर्देशिका को स्वयं शामिल करना है या नहीं। |

### प्रतिलाभ की मात्रा

Shar प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *directory* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है*directory*. |
| IOException | *directory* फ़ाइल के लिए खड़ा है, निर्देशिका के लिए नहीं। |

### उदाहरण

```csharp
using (FileStream sharFile = File.Open("archive.shar", FileMode.Create))
{
    using (var archive = new SharArchive())
    {
        archive.CreateEntries(new DirectoryInfo("C:\folder"), false);
        archive.Save(sharFile);
    }
}
```

### यह सभी देखें

* class [SharArchive](../)
* नाम स्थान [Aspose.Zip.Shar](../../shararchive/)
* सभा [Aspose.Zip](../../../)


