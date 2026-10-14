---
title: "IsoArchive.IsoArchive"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "IsoArchive कंस्ट्रक्टर। IsoArchive क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और नई फ़ाइलों और डायरेक्टरीज़ जोड़ने के लिए एक खाली ISO आर्काइव बनाता है।"
type: docs
weight: 10
url: /hi/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

[`IsoArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और नई फ़ाइलों और डायरेक्टरीज़ जोड़ने के लिए एक खाली ISO आर्काइव बनाता है।

```csharp
public IsoArchive()
```

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि कैसे एक नया खाली ISO आर्काइव बनाया जाए और उसमें फ़ाइलें जोड़ी जाएँ:

```csharp
// एक नया खाली ISO आर्काइव बनाएं
using(IsoArchive isoArchive = new IsoArchive())
{
    // ISO आर्काइव में फ़ाइलें जोड़ें
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // ISO आर्काइव को फ़ाइल में सहेजें
    isoArchive.Save("new_archive.iso");
}
```

### संबंधित देखें

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

[`IsoArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और आर्काइव से निकाले जा सकने वाली एंट्री सूची बनाता है।

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceStream | स्ट्रीम | आर्काइव का स्रोत। यह सर्चेबल होना चाहिए। |
| loadOptions | IsoLoadOptions | आर्काइव लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *sourceStream* null है। |
| ArgumentException | *sourceStream* सर्चेबल नहीं है। |
| InvalidDataException | *sourceStream* एक वैध ISO आर्काइव नहीं है। |
| ObjectDisposedException | यदि स्रोत स्ट्रीम को नष्ट कर दिया गया हो तो यह थ्रो किया जाता है। |
| EndOfStreamException | जब स्ट्रीम का अंत अप्रत्याशित रूप से पहुँच जाता है तो यह थ्रो किया जाता है। |
| IOException | एक I/O त्रुटि हुई। |
| NotSupportedException | स्ट्रीम पढ़ने का समर्थन नहीं करती। |

## टिप्पणियाँ

यह कंस्ट्रक्टर कोई भी एंट्री अनपैक नहीं करता।

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे एक्सट्रैक्ट किया जाए।

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### संबंधित देखें

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

[`IsoArchive`](../) क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है और आर्काइव से निकाले जा सकने वाली एंट्री सूची बनाता है।

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| पथ | String | आर्काइव फ़ाइल का पथ। |
| loadOptions | IsoLoadOptions | आर्काइव लोड करने के विकल्प। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉलर के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफ़ेद स्थान शामिल हैं, या इसमें अमान्य अक्षर हैं। |
| UnauthorizedAccessException | *path* फ़ाइल तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 अक्षरों से कम होने चाहिए, और फ़ाइल नाम 260 अक्षरों से कम होने चाहिए। |
| NotSupportedException | *path* पर फ़ाइल में स्ट्रिंग के मध्य में कोलन (:) है। |
| FileNotFoundException | फ़ाइल नहीं मिली। |
| DirectoryNotFoundException | निर्दिष्ट पथ अमान्य है, जैसे कि यह अनमैप्ड ड्राइव पर है। |
| IOException | फ़ाइल पहले से ही खुली है। |
| EndOfStreamException | फ़ाइल बहुत छोटी है। |
| InvalidDataException | जब डेटा अमान्य या भ्रष्ट हो तो फेंका जाता है। |

## टिप्पणियाँ

यह कंस्ट्रक्टर कोई भी एंट्री अनपैक नहीं करता।

## उदाहरण

निम्नलिखित उदाहरण दिखाता है कि सभी एंट्रीज़ को एक डायरेक्टरी में कैसे एक्सट्रैक्ट किया जाए।

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### संबंधित देखें

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


