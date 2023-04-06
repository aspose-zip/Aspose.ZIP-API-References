---
title: SevenZipArchive.SevenZipArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: SevenZipArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैSevenZipArchive इसक प्रवष्टयं के लए वैकल्पक सेटंग्स के सथ वर्ग
type: docs
weight: 10
url: /hi/net/aspose.zip.sevenzip/sevenziparchive/sevenziparchive/
---
## SevenZipArchive(SevenZipEntrySettings) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`SevenZipArchive`](../) इसकी प्रविष्टियों के लिए वैकल्पिक सेटिंग्स के साथ वर्ग।

```csharp
public SevenZipArchive(SevenZipEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| newEntrySettings | SevenZipEntrySettings | नए जोड़े गए संपीड़न और एन्क्रिप्शन सेटिंग्स के लिए उपयोग किया जाता है[`SevenZipArchiveEntry`](../../sevenziparchiveentry/) items. यदि निर्दिष्ट नहीं है, तो एन्क्रिप्शन के बिना LZMA संपीड़न का उपयोग किया जाएगा। |

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी एकल फ़ाइल को डिफ़ॉल्ट सेटिंग के साथ कैसे कंप्रेस करना है: एन्क्रिप्शन के बिना LZMA संपीड़न.

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
    using (var archive = new SevenZipArchive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(sevenZipFile);
    }
}
```

### यह सभी देखें

* class [SevenZipEntrySettings](../../../aspose.zip.saving/sevenzipentrysettings/)
* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## SevenZipArchive(Stream) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`SevenZipArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public SevenZipArchive(Stream sourceStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *sourceStream* खोजने योग्य नहीं है। |
| ArgumentNullException | *sourceStream* शून्य है। |
| NotImplementedException | पुरालेख में एक से अधिक कोडर हैं। अब केवल LZMA सम्पीडन समर्थित है। |

### टिप्पणियों

यह कंस्ट्रक्टर किसी प्रविष्टि को डिकम्प्रेस नहीं करता है। देखना[`ExtractToDirectory`](../extracttodirectory/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

```csharp
using (SevenZipArchive archive = new SevenZipArchive(File.OpenRead("archive.7z")))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### यह सभी देखें

* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)

---

## SevenZipArchive(string) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`SevenZipArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public SevenZipArchive(string path)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | पूरी तरह से योग्य या संग्रह फ़ाइल के सापेक्ष पथ। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path*, फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

यह कंस्ट्रक्टर किसी प्रविष्टि को डिकम्प्रेस नहीं करता है। देखना[`ExtractToDirectory`](../extracttodirectory/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

```csharp
using (SevenZipArchive archive = new SevenZipArchive("archive.7z"))
{
    archive.ExtractToDirectory("C:\\extracted");
}
```

### यह सभी देखें

* class [SevenZipArchive](../)
* नाम स्थान [Aspose.Zip.SevenZip](../../sevenziparchive/)
* सभा [Aspose.Zip](../../../)


