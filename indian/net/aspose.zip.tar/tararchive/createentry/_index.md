---
title: TarArchive.CreateEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: TarArchive तरक. संग्रह में एकल प्रवष्ट बनएं.
type: docs
weight: 80
url: /hi/net/aspose.zip.tar/tararchive/createentry/
---
## CreateEntry(string, Stream, FileSystemInfo) {#createentry_1}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public TarEntry CreateEntry(string name, Stream source, FileSystemInfo fileInfo = null)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| source | Stream | प्रविष्टि के लिए इनपुट स्ट्रीम। |
| fileInfo | FileSystemInfo | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा। |

### प्रतिलाभ की मात्रा

टार प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 मानक के अनुसार टार के लिए बहुत लंबा है। |
| ArgumentException | फ़ाइल का नाम, के एक भाग के रूप में*name*, 100 प्रतीकों से अधिक है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*fileInfo* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

*fileInfo* उल्लेख कर सकते हैंDirectoryInfo यदि प्रविष्टि निर्देशिका है।

### उदाहरण

```csharp
using (var archive = new TarArchive())
{
   archive.CreateEntry("bytes", new MemoryStream(new byte[] {0x00, 0xFF}));
   archive.Save(tarFile);
}
```

### यह सभी देखें

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public TarEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा। |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |

### प्रतिलाभ की मात्रा

टार प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| PathTooLongException | *name* IEEE 1003.1-1998 मानक के अनुसार टार के लिए बहुत लंबा है। |
| ArgumentException | फ़ाइल का नाम, के एक भाग के रूप में*name*, 100 प्रतीकों से अधिक है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*fileInfo* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

*fileInfo* उल्लेख कर सकते हैंDirectoryInfo यदि प्रविष्टि निर्देशिका है।

अगर फ़ाइल तुरंत खोली जाती है*openImmediately*संग्रह का निपटारा होने तक यह पैरामीटर अवरुद्ध हो जाता है।

### उदाहरण

```csharp
FileInfo fi = new FileInfo("data.bin");
using (var archive = new TarArchive())
{
   archive.CreateEntry("data.bin", fi);
   archive.Save(tarFile);
}
```

### यह सभी देखें

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public TarEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| path | String | फ़ाइल का पथ कंप्रेस किया जाना है. |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |

### प्रतिलाभ की मात्रा

टार प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *path* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *path* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। - या - फ़ाइल का नाम, के एक भाग के रूप में*name*, 100 प्रतीकों से अधिक है। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*path* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*path* , फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। - या -*name* IEEE 1003.1-1998 मानक के अनुसार टार के लिए बहुत लंबा है। |
| NotSupportedException | पर फाइल करें*path* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*path* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

अगर फ़ाइल तुरंत खोली जाती है*openImmediately*संग्रह का निपटारा होने तक यह पैरामीटर अवरुद्ध हो जाता है।

### उदाहरण

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save(outputTarFile);
}
```

### यह सभी देखें

* class [TarEntry](../../tarentry/)
* class [TarArchive](../)
* नाम स्थान [Aspose.Zip.Tar](../../tararchive/)
* सभा [Aspose.Zip](../../../)


