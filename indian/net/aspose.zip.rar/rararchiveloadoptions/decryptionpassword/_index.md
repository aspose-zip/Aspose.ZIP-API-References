---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: .NET API संदर्भ के लिए Aspose.ZIP
description: RarArchiveLoadOptions संपत्त. प्रवष्टयं और प्रवष्ट नमं क डक्रप्ट करने के लए पसवर्ड प्रप्त य सेट करत है
type: docs
weight: 20
url: /hi/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

प्रविष्टियों और प्रविष्टि नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त या सेट करता है।

```csharp
public string DecryptionPassword { get; set; }
```

### उदाहरण

आप आर्काइव निष्कर्षण पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.rar"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (RarArchive archive = new RarArchive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* नाम स्थान [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* सभा [Aspose.Zip](../../../)


