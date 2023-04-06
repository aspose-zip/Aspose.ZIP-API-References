---
title: ArchiveLoadOptions.Encoding
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveLoadOptions संपत्त. प्रवष्टयं के नमं के लए एन्कडंग प्रप्त य सेट करत है
type: docs
weight: 30
url: /hi/net/aspose.zip/archiveloadoptions/encoding/
---
## ArchiveLoadOptions.Encoding property

प्रविष्टियों के नामों के लिए एन्कोडिंग प्राप्त या सेट करता है।

```csharp
public Encoding Encoding { get; set; }
```

### उदाहरण

ज़िप फ़ाइल गुणों की परवाह किए बिना निर्दिष्ट एन्कोडिंग का उपयोग करके रचित प्रविष्टि नाम।

```csharp
using (FileStream fs = File.OpenRead("archive.zip"))
{      
    using (Archive archive = new Archive(fs, new ArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(932) }))
    {
        string name = archive.Entries[0].Name;
    }    
}
```

### यह सभी देखें

* class [ArchiveLoadOptions](../)
* नाम स्थान [Aspose.Zip](../../archiveloadoptions/)
* सभा [Aspose.Zip](../../../)


