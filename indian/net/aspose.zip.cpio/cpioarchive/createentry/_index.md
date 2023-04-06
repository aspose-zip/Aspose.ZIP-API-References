---
title: CpioArchive.CreateEntry
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: CpioArchive तरक. संग्रह में एकल प्रवष्ट बनएं.
type: docs
weight: 40
url: /hi/net/aspose.zip.cpio/cpioarchive/createentry/
---
## CreateEntry(string, FileInfo, bool) {#createentry}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public CpioEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| fileInfo | FileInfo | संपीड़ित की जाने वाली फ़ाइल या फ़ोल्डर का मेटाडेटा। |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |

### प्रतिलाभ की मात्रा

Cpio प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *name* शून्य है। |
| ArgumentException | *name* खाली है। |
| ArgumentNullException | *fileInfo* शून्य है। |

### टिप्पणियों

अगर फ़ाइल तुरंत खोली जाती है*openImmediately*संग्रह का निपटारा होने तक यह पैरामीटर अवरुद्ध हो जाता है।

### उदाहरण

```csharp
FileInfo fileInfo = new FileInfo("data.bin");
using (var archive = new CpioArchive())
{
    archive.CreateEntry("test.bin", fileInfo);
    archive.Save("archive.cpio");
}
```

### यह सभी देखें

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, string, bool) {#createentry_2}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public CpioEntry CreateEntry(string name, string sourcePath, bool openImmediately = false)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| sourcePath | String | फ़ाइल का पथ कंप्रेस किया जाना है. |
| openImmediately | Boolean | फ़ाइल को तुरंत खोलने पर सही, अन्यथा संग्रह सहेजने पर फ़ाइल खोलें. |

### प्रतिलाभ की मात्रा

Cpio प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *sourcePath* शून्य है। |
| SecurityException | कॉल करने वाले के पास एक्सेस करने के लिए आवश्यक अनुमति नहीं है। |
| ArgumentException | *sourcePath* खाली है, केवल सफेद स्थान हैं, या अमान्य वर्ण हैं। - या - फ़ाइल का नाम, के एक भाग के रूप में*name*, 100 प्रतीकों से अधिक है। |
| UnauthorizedAccessException | फ़ाइल तक पहुंच*sourcePath* वर्जित किया गया है। |
| PathTooLongException | विष्तृत*sourcePath* , फ़ाइल नाम, या दोनों सिस्टम-परिभाषित अधिकतम लंबाई से अधिक हैं। उदाहरण के लिए, Windows-आधारित प्लेटफ़ॉर्म पर, पथ 248 वर्णों से कम होने चाहिए और फ़ाइल नाम 260 वर्णों से कम होने चाहिए। - या -*name* सीपीओ के लिए बहुत लंबा है। |
| NotSupportedException | पर फाइल करें*sourcePath* स्ट्रिंग के बीच में एक कोलन (:) होता है। |

### टिप्पणियों

प्रवेश नाम पूरी तरह से भीतर सेट है*name* पैरामीटर। फ़ाइल नाम में प्रदान किया गया*sourcePath* पैरामीटर प्रविष्टि नाम को प्रभावित नहीं करता है।

अगर फ़ाइल तुरंत खोली जाती है*openImmediately*संग्रह का निपटारा होने तक यह पैरामीटर अवरुद्ध हो जाता है।

### उदाहरण

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### यह सभी देखें

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

संग्रह में एकल प्रविष्टि बनाएं.

```csharp
public CpioEntry CreateEntry(string name, Stream source)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| name | String | प्रविष्टि का नाम। |
| source | Stream | प्रविष्टि के लिए इनपुट स्ट्रीम। |

### प्रतिलाभ की मात्रा

Cpio प्रविष्टि उदाहरण।

### अपवाद

| अपवाद | स्थिति |
| --- | --- |
| ArgumentNullException | *name* शून्य है। |
| ArgumentNullException | *source* शून्य है। |
| ArgumentException | *name* खाली है। |

### उदाहरण

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("data.bin", File.OpenRead("data.bin"));
    archive.Save("archive.cpio");
}
```

### यह सभी देखें

* class [CpioEntry](../../cpioentry/)
* class [CpioArchive](../)
* नाम स्थान [Aspose.Zip.Cpio](../../cpioarchive/)
* सभा [Aspose.Zip](../../../)


