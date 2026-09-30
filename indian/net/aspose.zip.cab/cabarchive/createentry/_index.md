---
title: "CabArchive.CreateEntry"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "CabArchive मेथड। आर्काइव के भीतर एक एकल एंट्री बनाता है।"
type: docs
weight: 40
url: /hi/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| पथ | String | नए फ़ाइल का पूर्ण योग्य नाम, या संपीड़ित करने के लिए सापेक्ष फ़ाइल नाम। |
| newEntrySettings | CabEntrySettings | संपीड़न और एन्क्रिप्शन सेटिंग्स जो जोड़े गए [`CabEntry`](../../cabentry/) आइटम के लिए उपयोग की गई हैं। |

### रिटर्न वैल्यू

Cab एंट्री का उदाहरण।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए तैयार है और एंट्रीज़ नहीं जोड़ सकता। |

## टिप्पणियाँ

एंट्री नाम केवल *name* पैरामीटर के भीतर सेट किया जाता है। *path* पैरामीटर में दिया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

## उदाहरण

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### संबंधित देखें

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| स्रोत | स्ट्रीम | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| newEntrySettings | CabEntrySettings | संपीड़न और एन्क्रिप्शन सेटिंग्स जो जोड़े गए [`CabEntry`](../../cabentry/) आइटम के लिए उपयोग की गई हैं। |

### रिटर्न वैल्यू

Cab एंट्री का उदाहरण।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए तैयार है और एंट्रीज़ नहीं जोड़ सकता। |
| ArgumentNullException | *name* शून्य है। |

## उदाहरण

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### संबंधित देखें

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | संकुचित की जाने वाली फ़ाइल का मेटाडाटा। |
| newEntrySettings | CabEntrySettings | संपीड़न और एन्क्रिप्शन सेटिंग्स जो जोड़े गए [`CabEntry`](../../cabentry/) आइटम के लिए उपयोग की गई हैं। |

### रिटर्न वैल्यू

CAB एंट्री का उदाहरण।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* केवल-पढ़ने योग्य है या यह एक निर्देशिका है। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| FileNotFoundException | *fileInfo* एक ऐसी फ़ाइल को दर्शाता है जिसे नहीं मिला। |
| SecurityException | कॉलर के पास *fileInfo* तक पहुंचने के लिए आवश्यक अनुमति नहीं है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए तैयार है और एंट्रीज़ नहीं जोड़ सकता। |
| ArgumentNullException | *name* शून्य है। |

## टिप्पणियाँ

एंट्री नाम केवल *name* पैरामीटर के भीतर सेट किया जाता है। *fileInfo* पैरामीटर में दिया गया फ़ाइल नाम एंट्री नाम को प्रभावित नहीं करता।

## उदाहरण

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### संबंधित देखें

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

आर्काइव के भीतर एक एकल एंट्री बनाएं।

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| streamProvider | Func`1 | एंट्री के लिए इनपुट स्ट्रीम प्रदान करने वाली विधि। |
| newEntrySettings | CabEntrySettings | संपीड़न और एन्क्रिप्शन सेटिंग्स जो जोड़े गए [`CabEntry`](../../cabentry/) आइटम के लिए उपयोग की गई हैं। |

### रिटर्न वैल्यू

CAB एंट्री का उदाहरण।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| InvalidOperationException | आर्काइव डिकम्प्रेशन के लिए बनाया गया है। - या - फ़ाइलों की संख्या सीमा तक पहुँच गई है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentException | *name* शून्य या खाली है। |

## उदाहरण

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### संबंधित देखें

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


