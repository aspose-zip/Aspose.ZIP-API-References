---
title: "XarArchive.CreateEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "XarArchive मेथड। आर्काइव के भीतर एक एकल एंट्री बनाता है।"
type: docs
weight: 40
url: /hi/net/aspose.zip.xar/xararchive/createentry/
---
## CreateEntry(string, FileInfo, bool, XarCompressionSettings) {#createentry}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public XarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | कम्प्रेस की जाने वाली फ़ाइल या फ़ोल्डर की मेटाडेटा। |
| openImmediately | Boolean | सही, यदि फ़ाइल को तुरंत खोला जाए, अन्यथा संग्रह सहेजते समय फ़ाइल को खोला जाएगा। |
| compressionSettings | XarCompressionSettings | जोड़े गए [`XarEntry`](../../xarentry/) आइटम के लिए उपयोग किए गए कम्प्रेशन सेटिंग्स। |

### रिटर्न वैल्यू

Xar एंट्री इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *name* शून्य है। |
| ArgumentException | *name* खाली है। |
| ArgumentNullException | *fileInfo* शून्य है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

यदि फ़ाइल को *openImmediately* पैरामीटर के साथ तुरंत खोला जाता है तो यह आर्काइव के डिस्पोज़ होने तक ब्लॉक हो जाता है।

## उदाहरण

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new XarArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.xar");
}
```

### संबंधित देखें

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool, XarCompressionSettings) {#createentry_2}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public XarEntry CreateEntry(string name, string sourcePath, bool openImmediately = false, 
    XarCompressionSettings compressionSettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| sourcePath | String | संकुचित करने वाली फ़ाइल का पथ। |
| openImmediately | Boolean | सही, यदि फ़ाइल को तुरंत खोला जाए, अन्यथा संग्रह सहेजते समय फ़ाइल को खोला जाएगा। |
| compressionSettings | XarCompressionSettings | जोड़े गए [`XarEntry`](../../xarentry/) आइटम के लिए उपयोग किए गए कम्प्रेशन सेटिंग्स। |

### रिटर्न वैल्यू

Xar एंट्री इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *sourcePath* null है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *sourcePath* खाली है, केवल खाली स्थान शामिल करता है, या अवैध अक्षर शामिल हैं। - या - फ़ाइल नाम, *name* का भाग, 100 प्रतीकों से अधिक है। |
| UnauthorizedAccessException | फ़ाइल *sourcePath* तक पहुंच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *sourcePath*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। - या - *name* xar के लिए बहुत लंबा है। |
| NotSupportedException | फ़ाइल *sourcePath* में स्ट्रिंग के मध्य में कोलन (:) है। |
| InvalidOperationException | xar संग्रह को संशोधित करना असंभव है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## टिप्पणियाँ

एंट्री नाम केवल *name* पैरामीटर में सेट किया जाता है। *sourcePath* पैरामीटर में दिया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

यदि फ़ाइल को *openImmediately* पैरामीटर के साथ तुरंत खोला जाता है तो यह आर्काइव के डिस्पोज़ होने तक ब्लॉक हो जाता है।

## उदाहरण

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.xar");
}
```

### संबंधित देखें

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, XarCompressionSettings) {#createentry_1}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public XarEntry CreateEntry(string name, Stream source, 
    XarCompressionSettings compressionSettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| स्रोत | स्ट्रीम | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| compressionSettings | XarCompressionSettings | जोड़े गए [`XarEntry`](../../xarentry/) आइटम के लिए उपयोग किए गए कम्प्रेशन सेटिंग्स। |

### रिटर्न वैल्यू

Xar एंट्री इंस्टेंस।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *name* शून्य है। |
| ArgumentNullException | *source* null है। |
| ArgumentException | *name* खाली है। |
| InvalidOperationException | xar संग्रह को संशोधित करना असंभव है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |

## उदाहरण

```csharp
using (var archive = new XarArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.xar");
}
```

### संबंधित देखें

* class [XarEntry](../../xarentry/)
* class [XarCompressionSettings](../../xarcompressionsettings/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


