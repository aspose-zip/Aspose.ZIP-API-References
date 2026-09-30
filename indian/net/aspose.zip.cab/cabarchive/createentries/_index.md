---
title: "CabArchive.CreateEntries"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "CabArchive मेथड। निर्दिष्ट निर्देशिका से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.cab/cabarchive/createentries/
---
## CreateEntries(DirectoryInfo, bool) {#createentries}

निर्दिष्ट निर्देशिका से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```csharp
public CabArchive CreateEntries(DirectoryInfo directory, bool includeRootDirectory = true)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| directory | DirectoryInfo | संकुचित करने के लिए निर्देशिका। |
| includeRootDirectory | Boolean | यह दर्शाता है कि एंट्री पाथ में रूट निर्देशिका का नाम शामिल करना है या नहीं। |

### रिटर्न वैल्यू

वर्तमान [`CabArchive`](../) उदाहरण।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | *directory* शून्य है। |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| DirectoryNotFoundException | *directory* नहीं मिला। |
| SecurityException | कॉलर के पास *directory* या उसकी सामग्री तक पहुंचने के लिए आवश्यक अनुमति नहीं है। |
| UnauthorizedAccessException | *directory* या उसकी किसी फ़ाइल तक पहुंच अस्वीकृत है। |
| IOException | एक I/O त्रुटि *directory* तक पहुँचते समय होती है। |
| PathTooLongException | जनरेट किया गया एंट्री पाथ सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए तैयार है और एंट्रीज़ नहीं जोड़ सकता। |

## उदाहरण

```csharp
using (var archive = new CabArchive())
{
    var directory = new DirectoryInfo("logs");
    archive.CreateEntries(directory);
    archive.Save("logs.cab");
}
```

### संबंधित देखें

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntries(string, bool) {#createentries_1}

निर्दिष्ट डायरेक्टरी पाथ से सभी फ़ाइलों को पुनरावर्ती रूप से आर्काइव में जोड़ता है।

```csharp
public CabArchive CreateEntries(string sourceDirectory, bool includeRootDirectory = true)
```

| पैरामीटर | टाइप | विवरण |
| --- | --- | --- |
| sourceDirectory | String | कम्प्रेस करने के लिए डायरेक्टरी पाथ। |
| includeRootDirectory | Boolean | यह दर्शाता है कि एंट्री पाथ में रूट निर्देशिका का नाम शामिल करना है या नहीं। |

### रिटर्न वैल्यू

वर्तमान [`CabArchive`](../) उदाहरण।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ObjectDisposedException | आर्काइव को नष्ट कर दिया गया है और इसे उपयोग नहीं किया जा सकता। |
| ArgumentNullException | *sourceDirectory* शून्य है। |
| DirectoryNotFoundException | *sourceDirectory* नहीं मिला। |
| SecurityException | कॉलर के पास *sourceDirectory* तक पहुँचने के लिए आवश्यक अनुमति नहीं है। |
| UnauthorizedAccessException | *sourceDirectory* तक पहुँच अस्वीकृत है। |
| PathTooLongException | निर्दिष्ट *sourceDirectory* सिस्टम-परिभाषित अधिकतम लंबाई से अधिक है। |
| ArgumentException | *sourceDirectory* खाली है, केवल व्हाइटस्पेस शामिल है, या अमान्य अक्षर हैं। |
| IOException | एक I/O त्रुटि *sourceDirectory* तक पहुँचते समय होती है। |
| InvalidOperationException | आर्काइव निष्कर्षण के लिए तैयार है और एंट्रीज़ नहीं जोड़ सकता। |

## उदाहरण

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabStoreCompressionSettings())))
{
    archive.CreateEntries("data", includeRootDirectory: false);
    archive.Save("stored_data.cab");
}
```

### संबंधित देखें

* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


