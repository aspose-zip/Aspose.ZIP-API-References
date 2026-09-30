---
title: "XarArchive.CreateEntries"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarArchive मेथड। दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावृत्त रूप से संग्रह में जोड़ता है।"
type: docs
weight: 30
url: /hi/net/aspose.zip.xar/xararchive/createentries/
---
## CreateEntries(string, bool, XarCompressionSettings) {#createentries_1}

दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावृत्त रूप से संग्रह में जोड़ता है।

```csharp
public XarArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceDirectory | String | संकुचित करने के लिए निर्देशिका। |
| compressionSettings | Boolean | जोड़े गए [`XarEntry`](../../xarentry/) आइटमों के लिए उपयोग किए गए संपीड़न सेटिंग्स। |
| includeRootDirectory | XarCompressionSettings | निर्देशित करता है कि मूल निर्देशिका को स्वयं शामिल किया जाए या नहीं। |

### रिटर्न वैल्यू

Xar एंट्री इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *sourceDirectory* शून्य है। |
| SecurityException | कॉलर के पास *sourceDirectory* तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *sourceDirectory* में अवैध अक्षर हैं जैसे ", &lt;, &gt;, या &#x7C;। |
| PathTooLongException | निर्दिष्ट पथ, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। निर्दिष्ट पथ, फ़ाइल नाम, या दोनों बहुत लंबे हैं। |
| IOException | *sourceDirectory* एक फ़ाइल को दर्शाता है, निर्देशिका नहीं। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(@"C:\folder", false);
        archive.Save(xarFile);
    }
}
```

### संबंधित देखें

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(DirectoryInfo, bool, XarCompressionSettings) {#createentries}

दिए गए निर्देशिका में सभी फ़ाइलों और निर्देशिकाओं को पुनरावृत्त रूप से संग्रह में जोड़ता है।

```csharp
public XarArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true, 
    XarCompressionSettings compressionSettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| directory | DirectoryInfo | संकुचित करने के लिए निर्देशिका। |
| compressionSettings | Boolean | जोड़े गए [`XarEntry`](../../xarentry/) आइटमों के लिए उपयोग किए गए संपीड़न सेटिंग्स। |
| includeRootDirectory | XarCompressionSettings | निर्देशित करता है कि मूल निर्देशिका को स्वयं शामिल किया जाए या नहीं। |

### रिटर्न वैल्यू

Xar एंट्री इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *directory* शून्य है। |
| SecurityException | कॉलर के पास *directory* तक पहुंचने की आवश्यक अनुमति नहीं है। |
| IOException | *directory* एक फ़ाइल को दर्शाता है, निर्देशिका नहीं। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

```csharp
using (FileStream xarFile = File.Open("archive.xar", FileMode.Create))
{
    using (var archive = new XarArchive())
    {
        archive.CreateEntries(new DirectoryInfo(@"C:\folder"), false);
        archive.Save(xarFile);
    }
}
```

### संबंधित देखें

* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


