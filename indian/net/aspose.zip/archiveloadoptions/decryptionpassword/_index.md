---
title: ArchiveLoadOptions.DecryptionPassword
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: ArchiveLoadOptions संपत्त. डक्रप्ट प्रवष्टयं के लए पसवर्ड प्रप्त करत है य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

डिक्रिप्ट प्रविष्टियों के लिए पासवर्ड प्राप्त करता है या सेट करता है।

```csharp
public string DecryptionPassword { get; set; }
```

### उदाहरण

आप आर्काइव निष्कर्षण पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.zip"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
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
    }
}
```

### यह सभी देखें

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* नाम स्थान [Aspose.Zip](../../archiveloadoptions/)
* सभा [Aspose.Zip](../../../)


