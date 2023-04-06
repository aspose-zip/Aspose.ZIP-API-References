---
title: RarArchive.RarArchive
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: RarArchive नर्मत. क एक नय उदहरण प्ररंभ करत हैRarArchive क्लस और कंपज़ एंट्र लस्ट क आर्कइव से नकल ज सकत है
type: docs
weight: 10
url: /hi/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`RarArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| path | String | पूरी तरह से योग्य या संग्रह फ़ाइल के सापेक्ष पथ। |
| loadOptions | RarArchiveLoadOptions | मौजूदा संग्रह को लोड करने के विकल्प। |

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

यह कंस्ट्रक्टर किसी प्रविष्टि को डिकम्प्रेस नहीं करता है। देखना[`Open`](../../rararchiveentry/open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

निम्न उदाहरण एक आर्काइव को एक्सट्रेक्ट करता है, फिर a में पहली प्रविष्टि को डिकम्प्रेस करता है`मेमोरीस्ट्रीम`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* नाम स्थान [Aspose.Zip.Rar](../../rararchive/)
* सभा [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`RarArchive`](../) क्लास और कंपोज़ एंट्री लिस्ट को आर्काइव से निकाला जा सकता है।

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| sourceStream | Stream | संग्रह का स्रोत। |
| loadOptions | RarArchiveLoadOptions | मौजूदा संग्रह को लोड करने के विकल्प। |

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentException | *sourceStream* खोजने योग्य नहीं है। |
| InvalidDataException | संग्रह के लिए गलत हस्ताक्षर। - या - फ़ाइल RAR संग्रह नहीं है। |
| InvalidOperationException |  |

### टिप्पणियों

यह कंस्ट्रक्टर किसी प्रविष्टि को डिकम्प्रेस नहीं करता है। देखना[`Open`](../../rararchiveentry/open/) डीकंप्रेसिंग के लिए विधि.

### उदाहरण

निम्नलिखित उदाहरण पहली प्रविष्टि को डिक्रिप्ट और डिकम्प्रेस करता है`मेमोरीस्ट्रीम`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* नाम स्थान [Aspose.Zip.Rar](../../rararchive/)
* सभा [Aspose.Zip](../../../)


