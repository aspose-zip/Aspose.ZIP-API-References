---
title: Archive.Archive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: Archive नर्मत. क एक नय उदहरण प्ररंभ करत हैArchive इसक प्रवष्टयं के लए वैकल्पक सेटंग्स के सथ वर्ग
type: docs
weight: 10
url: /hi/net/aspose.zip/archive/archive/
---
## Archive(ArchiveEntrySettings) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`Archive`](../) इसकी प्रविष्टियों के लिए वैकल्पिक सेटिंग्स के साथ वर्ग।

```csharp
public Archive(ArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| newEntrySettings | ArchiveEntrySettings | नए जोड़े गए संपीड़न और एन्क्रिप्शन सेटिंग्स के लिए उपयोग किया जाता है[`ArchiveEntry`](../../archiveentry/) items. यदि निर्दिष्ट नहीं है, तो एन्क्रिप्शन के बिना सबसे सामान्य डिफ्लेट संपीड़न का उपयोग किया जाएगा। |

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी एकल फ़ाइल को डिफ़ॉल्ट सेटिंग के साथ कैसे कंप्रेस करना है.

```csharp
using (FileStream zipFile = File.Open("archive.zip", FileMode.Create))
{
    using (var archive = new Archive())
    {
        archive.CreateEntry("data.bin", "file.dat");
        archive.Save(zipFile);
    }
}
```

### यह सभी देखें

* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## Archive(Stream, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Archive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public Archive(Stream sourceStream, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। |
| loadOptions | ArchiveLoadOptions | मौजूदा संग्रह को लोड करने के विकल्प। |
| newEntrySettings | ArchiveEntrySettings | नए जोड़े गए संपीड़न और एन्क्रिप्शन सेटिंग्स के लिए उपयोग किया जाता है[`ArchiveEntry`](../../archiveentry/) items. यदि निर्दिष्ट नहीं है, तो एन्क्रिप्शन के बिना सबसे सामान्य डिफ्लेट संपीड़न का उपयोग किया जाएगा। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *sourceStream* खोजने योग्य नहीं है। |
| InvalidDataException | एईएस के लिए एन्क्रिप्शन शीर्षलेख WinZip संपीड़न विधि का खंडन करता है। |

### टिप्पणियों

यह कंस्ट्रक्टर किसी प्रविष्टि को डिकम्प्रेस नहीं करता है। देखना[`Open`](../../archiveentry/open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण एक एन्क्रिप्टेड आर्काइव को एक्सट्रेक्ट करता है, फिर पहली प्रविष्टि को डीकंप्रेस करता है`मेमोरीस्ट्रीम`.

```csharp
var fs = File.OpenRead("encrypted.zip");
var extracted = new MemoryStream();
using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### यह सभी देखें

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)

---

## Archive(string, ArchiveLoadOptions, ArchiveEntrySettings) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`Archive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public Archive(string path, ArchiveLoadOptions loadOptions = null, 
    ArchiveEntrySettings newEntrySettings = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | पूरी तरह से योग्य या संग्रह फ़ाइल के सापेक्ष पथ। |
| loadOptions | ArchiveLoadOptions | मौजूदा संग्रह को लोड करने के विकल्प। |
| newEntrySettings | ArchiveEntrySettings | नए जोड़े गए संपीड़न और एन्क्रिप्शन सेटिंग्स के लिए उपयोग किया जाता है[`ArchiveEntry`](../../archiveentry/) items. यदि निर्दिष्ट नहीं है, तो एन्क्रिप्शन के बिना सबसे सामान्य डिफ्लेट संपीड़न का उपयोग किया जाएगा। |

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

यह कंस्ट्रक्टर किसी प्रविष्टि को डिकम्प्रेस नहीं करता है। देखना[`Open`](../../archiveentry/open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण एक एन्क्रिप्टेड आर्काइव को एक्सट्रेक्ट करता है, फिर पहली प्रविष्टि को डीकंप्रेस करता है`मेमोरीस्ट्रीम`.

```csharp
var extracted = new MemoryStream();
using (Archive archive = new Archive("encrypted.zip", new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### यह सभी देखें

* class [ArchiveLoadOptions](../../archiveloadoptions/)
* class [ArchiveEntrySettings](../../../aspose.zip.saving/archiveentrysettings/)
* class [Archive](../)
* नाम स्थान [Aspose.Zip](../../archive/)
* सभा [Aspose.Zip](../../../)


