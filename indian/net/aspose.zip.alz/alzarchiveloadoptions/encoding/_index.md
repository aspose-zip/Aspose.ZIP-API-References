---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AlzArchiveLoadOptions प्रॉपर्टी। एंट्री नामों के लिए एन्कोडिंग प्राप्त या सेट करती है। डिफ़ॉल्ट कोरियन विंडोज कोड पेज 949 CP949 है।"
type: docs
weight: 40
url: /hi/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

एंट्रीज़ के नामों के लिए एन्कोडिंग प्राप्त करता है या सेट करता है। डिफ़ॉल्ट कोरियाई विंडोज कोड पेज 949 (CP949) है।

```csharp
public Encoding Encoding { get; set; }
```

## टिप्पणियाँ

ALZ आर्काइव्स ऐतिहासिक रूप से फ़ाइल नामों को कोरियन विंडोज ANSI कोड पेज का उपयोग करके संग्रहीत करते हैं।

## उदाहरण

निर्दिष्ट एन्कोडिंग का उपयोग करके एंट्री नाम बनाया गया है।

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### संबंधित देखें

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


